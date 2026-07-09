# Code Review Checklist Reference

This checklist contains the authoritative standards applied by the `code-reviewer` skill. Use this to audit files, diffs, or PRs.

---

## 1. Correctness
*Does the code behave correctly and reliably under all expected conditions?*

- [ ] **Functional Match:** Does the code implement all requirements of the task/feature accurately?
- [ ] **Edge Cases:** Are boundary conditions handled properly (e.g., empty arrays, null values, negative numbers, extreme inputs)?
- [ ] **Logical Faults:** Are there any logical errors, off-by-one errors, infinite loops, or incorrect state transformations?
- [ ] **Resource Cleanup:** Are resources (file handles, database connections, sockets, streams) closed correctly in both success and error blocks?
- [ ] **Concurrency:** If the code is multi-threaded or async, are there potential race conditions, deadlocks, or state corruption?

---

## 2. Security
*Is the code free of common vulnerabilities and design flaws?*

- [ ] **Input Validation:** Is all external input (parameters, request bodies, query strings, headers) sanitized and validated?
- [ ] **Credentials & Secrets:** Are passwords, API keys, tokens, or personal identifiers hard-coded, committed, or written to logs?
- [ ] **Authorization:** Are authentication and authorization checks enforced at every entry point and API route boundary?
- [ ] **Injection Prevention:** Are queries parameterized to prevent SQL, NoSQL, command, or shell injections?
- [ ] **Cryptography:** Are secure, modern cryptographic algorithms and libraries used (e.g., no MD5/SHA-1 for password hashing, cryptographically secure randoms)?

---

## 3. Performance
*Is the code optimized for speed, memory efficiency, and resource utilization?*

- [ ] **Algorithm Complexity:** Are algorithmic choices optimal for the expected input size (e.g., avoiding $O(N^2)$ inside loops)?
- [ ] **Database Operations:** Are database queries indexed? Is the N+1 query problem avoided? Are large datasets queried with limits and pagination?
- [ ] **Memory Management:** Are large objects or memory buffers handled efficiently without leaking memory?
- [ ] **Caching:** Are expensive computations or frequently retrieved, static data cached where appropriate?
- [ ] **Network & I/O:** Are roundtrips minimized (e.g., batching API requests)? Are operations non-blocking/asynchronous where possible?

---

## 4. Maintainability & Code Quality
*Is the code clean, readable, modular, and easy to modify?*

- [ ] **Naming Conventions:** Are variable, function, class, and file names self-documenting and consistent with the codebase?
- [ ] **DRY (Don't Repeat Yourself):** Is duplicate code refactored into reusable functions, helper modules, or libraries?
- [ ] **Single Responsibility Principle:** Does each function, class, or module have one clear, well-defined purpose?
- [ ] **Magic Values:** Are magic numbers, strings, or boolean flags extracted into named constants or configuration settings?
- [ ] **Size & Complexity:** Are functions kept short (under 30-50 lines)? Are complex code nesting levels minimized?

---

## 5. Architecture & Design
*Does the code align with the broader project design and clean coding principles?*

- [ ] **Design Patterns:** Does the design align with existing architectural conventions (e.g., MVC, Layered architecture, Hexagonal)?
- [ ] **Separation of Concerns:** Is there a clear boundary between presentation/UI, business logic, data access, and infrastructure?
- [ ] **Unnecessary Coupling:** Are components loosely coupled, allowing them to be modified or replaced independently?
- [ ] **API Design:** Are API routes, request payloads, response schemas, and HTTP status codes RESTful and clean?

---

## 6. Testing
*Is the code properly validated by unit, integration, and end-to-end tests?*

- [ ] **Test Coverage:** Are critical paths, business rules, and error conditions tested?
- [ ] **Test Design:** Are unit tests fast, isolated, and free of external dependencies (e.g., databases, external APIs)?
- [ ] **Mocking Boundaries:** Are external systems mocked at the boundary? Are mock data and factories structured realistically?
- [ ] **Test Assertions:** Are test expectations specific and asserting behavior rather than internal implementation details?

---

## 7. Error Handling & Resilience
*Does the system handle errors gracefully without crashing or leaking details?*

- [ ] **Catch Blocks:** Are catch blocks catching specific error types? (Avoid empty catch blocks `catch {}`).
- [ ] **Graceful Failures:** If a non-critical component fails (e.g., analytics, side-panel load), does the rest of the application continue to function?
- [ ] **User Feedback:** Are errors translated into user-friendly, descriptive messages instead of technical stack traces?
- [ ] **Retries & Timeouts:** Are network requests configured with appropriate timeouts and retry strategies (with backoff)?

---

## 8. Documentation
*Is the documentation up-to-date and helpful for future developers?*

- [ ] **Inline Comments:** Are complex algorithms, mathematical logic, or non-obvious design workarounds explained in inline comments?
- [ ] **Public APIs:** Are public APIs, functions, components, and classes documented using JSDoc, Docstrings, or corresponding style standard?
- [ ] **Changelog / Readme:** Are changes documented in relevant markdown files or the release notes if required?
