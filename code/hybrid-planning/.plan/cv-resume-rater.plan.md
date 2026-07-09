# Plan: CV & Resume Rater (Client-Side Only)

**Version:** 1.0
**Status:** COMPLETE
**Created:** 2026-05-30
**Estimated Steps:** 8

---

## 1. Context & Goals

> Develop a client-side only Vue 3 application that allows users to upload their CV/Resume (PDF format) and receive an instant rating and feedback. Since there is no backend, all file processing (text extraction) and analysis (heuristic scoring based on keywords, length, and formatting rules) will happen securely in the user's browser. The goal is to provide a polished, interactive, and visually appealing UI with rich feedback states.

**Out of Scope:**

- Server-side processing, file uploading to a server, or data storage.
- DOCX parsing (v1 focuses on PDF via `pdfjs-dist`).
- Real LLM integration (uses a localized heuristic ruleset to simulate AI rating to remain strictly local).

---

## 2. Affected Files Map

### Created

- `.plan/cv-resume-rater.plan.md` — This plan document.
- `package.json` — Vue project dependencies (Vue 3, Vite, pdfjs-dist).
- `index.html` — Main HTML entry point.
- `vite.config.js` — Vite configuration.
- `src/main.js` — Vue app entry point.
- `src/App.vue` — Main layout and state container.
- `src/assets/style.css` — Vanilla CSS styling (variables, animations, layout).
- `src/components/DropZone.vue` — Drag & Drop file uploader.
- `src/components/AnalysisLoader.vue` — Animated loading state.
- `src/components/ResultDashboard.vue` — Displays the score, pros, cons, and keywords.
- `src/services/pdfParser.js` — Client-side PDF text extraction logic.
- `src/services/heuristicRater.js` — Logic to score the extracted text.

### Modified

_(None - Greenfield project)_

### Deleted

_(None)_

---

## 3. Architectural Design

### 3.1 Component / Module Hierarchy

```text
App.vue (Holds active state: 'upload' | 'analyzing' | 'result')
 ├── DropZone.vue (Handles file input, emits 'file-selected')
 ├── AnalysisLoader.vue (Shows progress steps to simulate deep AI thought)
 └── ResultDashboard.vue (Receives analysis data, renders score ring & feedback)
```

### 3.2 State Management (Composition API)

- `appState`: ref<'upload' | 'analyzing' | 'result'>
- `cvData`: ref<null | File>
- `analysisResult`: ref<null | RatingResult>

### 3.3 Data Layer (Local Services)

- **`pdfParser.js`**: Wraps `pdfjs-dist` to convert an ArrayBuffer to a raw string.
- **`heuristicRater.js`**: Analyzes the string for:
    - **Action verbs** (e.g., "managed", "developed", "led").
    - **Quantifiable metrics** (e.g., "%", "$", numbers).
    - **Contact Info** (regex for email, phone).
    - **Length** (word count bounds).

---

## 4. Strict Contract Definitions

### 4.1 TypeScript Interfaces & Types (Documented for Vue JS)

```javascript
/**
 * @typedef {Object} RatingResult
 * @property {number} score - Overall score 0-100
 * @property {string[]} pros - List of strong points found
 * @property {string[]} cons - List of areas to improve
 * @property {string[]} keywords - Key skills extracted
 * @property {object} metrics
 * @property {number} metrics.wordCount
 * @property {boolean} metrics.hasContactInfo
 * @property {number} metrics.actionVerbsCount
 */
```

---

## 5. Edge Cases & Security Audit

| #   | Scenario                             | Expected Behavior                    | Mitigation                                                   |
| --- | ------------------------------------ | ------------------------------------ | ------------------------------------------------------------ |
| 1   | Uploading non-PDF file               | Reject file with error UI            | Input `accept=".pdf"` + client-side validation.              |
| 2   | Extremely large PDF                  | Reject if > 5MB to prevent UI freeze | Size check in DropZone.                                      |
| 3   | PDF with no extractable text (image) | Score drops, add specific "con"      | Detect low word count, prompt user to use text-based PDF.    |
| 4   | XSS via CV Text in UI                | Safely bind text in DOM              | Vue's default `{{ }}` interpolation prevents HTML injection. |

---

## 6. Step-by-Step Execution Checklist

- [x] **Step 1** — Initialize the project structure using Vite (Vue template), clear boilerplate, and install `pdfjs-dist`.
- [x] **Step 2** — `src/assets/style.css` — Setup global CSS variables for a modern, rich aesthetic (colors, spacing, shadows, keyframe animations).
- [x] **Step 3** — `src/services/pdfParser.js` — Implement PDF to text extraction using `pdfjs-dist`.
- [x] **Step 4** — `src/services/heuristicRater.js` — Build the mock AI scoring engine returning the `RatingResult` object.
- [x] **Step 5** — `src/components/DropZone.vue` — Build the drag-and-drop file upload UI.
- [x] **Step 6** — `src/components/AnalysisLoader.vue` — Build a compelling animated loading screen.
- [x] **Step 7** — `src/components/ResultDashboard.vue` — Build the score visualization (circular progress) and feedback lists.
- [x] **Step 8** — `src/App.vue` — Wire the components together and handle the application state flow.

---

## 7. Rollback Plan

- **Files to delete:** `src/*`, `index.html`, `vite.config.js`, `package.json`.
- Delete project files and restart Vite initialization if core dependencies fail.

---

## 8. Validation Criteria

- [ ] The app runs successfully on `npm run dev`.
- [ ] A user can drag and drop a PDF file.
- [ ] The application extracts text locally (observable via network tab showing no outbound data).
- [ ] A score between 0 and 100 is presented alongside actionable feedback.
- [ ] The UI feels modern and responsive using vanilla CSS.
