# Tech Stack Recommendations by Product Type

When the user hasn't specified a stack, use this guide to recommend one based on their product type.
Always explain WHY you're recommending a stack — don't just list technologies.

---

## How to Use This File

1. Identify the product type from the interview
2. Find the matching category below
3. Recommend the primary stack with brief rationale
4. Note the alternatives and when to consider them

---

## Web App (B2C / Consumer SaaS)

**Recommended Stack: Next.js Full-Stack**

| Layer          | Technology                               | Why                                                     |
| -------------- | ---------------------------------------- | ------------------------------------------------------- |
| Frontend + SSR | Next.js 14+ (App Router)                 | SEO, performance, DX, huge ecosystem                    |
| Language       | TypeScript                               | Type safety, fewer runtime bugs                         |
| UI             | Tailwind CSS + shadcn/ui                 | Fast to build, consistent, accessible by default        |
| State          | TanStack Query + Zustand                 | Async state vs. client state, separated concerns        |
| Auth           | Clerk or Auth0                           | Battle-tested, social login, MFA, saves weeks           |
| Database       | PostgreSQL (via Supabase or Neon)        | Relational, reliable, JSON support, serverless-friendly |
| ORM            | Drizzle ORM                              | Typesafe, lightweight, great with serverless            |
| Hosting        | Vercel (frontend) + Railway/Render (API) | Zero-config deploys, great DX                           |
| Email          | Resend                                   | Modern API, great React Email support                   |
| File Storage   | Cloudflare R2                            | Cheap, S3-compatible, no egress fees                    |
| Analytics      | PostHog                                  | Open source, product analytics + session replay         |
| Error Tracking | Sentry                                   | Industry standard                                       |

**When to use:** Consumer products, marketing-heavy apps, content-driven products, anything needing SEO.

**Alternative for simpler products:** Next.js with Supabase as backend (BaaS) — skip the custom API entirely.

---

## B2B SaaS / Dashboard-heavy Apps

**Recommended Stack: React + Dedicated Backend**

| Layer           | Technology                        | Why                                                     |
| --------------- | --------------------------------- | ------------------------------------------------------- |
| Frontend        | React 18+ (Vite) or Next.js       | SPA appropriate for app-like UIs                        |
| Language        | TypeScript                        | Essential for large codebases                           |
| UI              | shadcn/ui + Radix + Tailwind      | Accessible components, full control                     |
| Data Tables     | TanStack Table                    | Best-in-class, headless                                 |
| State           | TanStack Query + Zustand          | Same as above                                           |
| Backend         | Node.js + Fastify or NestJS       | Fastify: high performance; NestJS: structured for teams |
| Auth            | Auth0 or Clerk (with org support) | Multi-tenancy, SSO, SCIM, RBAC out of the box           |
| Database        | PostgreSQL + Redis                | RDBMS for core data, Redis for sessions/cache           |
| ORM             | Prisma or Drizzle                 | Prisma: more tooling; Drizzle: lighter, faster          |
| Background Jobs | BullMQ (via Redis)                | Battle-tested queue system                              |
| Hosting         | AWS ECS / GCP Cloud Run / Fly.io  | More control, better for variable load                  |

**When to use:** Admin panels, internal tools, multi-tenant SaaS, compliance-heavy industries.

**Alternative:** NestJS (more opinionated, better for larger teams with structure requirements).

---

## Mobile App (iOS + Android)

**Recommended Stack: React Native + Expo**

| Layer              | Technology                      | Why                                       |
| ------------------ | ------------------------------- | ----------------------------------------- |
| Framework          | React Native via Expo           | Write once, iOS + Android, huge ecosystem |
| Language           | TypeScript                      | Same as web, team can share knowledge     |
| Navigation         | Expo Router (file-based)        | Natural for React developers              |
| UI                 | NativeWind + custom components  | Tailwind-like syntax for mobile           |
| State              | TanStack Query + Zustand        | Same pattern as web                       |
| Auth               | Clerk or Supabase Auth          | Native-friendly SDKs                      |
| Backend            | Same as above (REST or GraphQL) | Share backend with web if applicable      |
| Push Notifications | Expo Notifications              | Cross-platform, simple                    |
| OTA Updates        | Expo Updates / EAS Update       | Ship fixes without app store review       |
| CI/CD              | EAS Build                       | Managed iOS/Android build service         |

**When to use:** Consumer mobile products, products where offline capability matters, MVP.

**Alternative:** Flutter — better performance, wider platform reach (web/desktop too), but requires Dart knowledge.

---

## API-Only / Backend Service

**Recommended Stack: Node.js or Python**

### Node.js (when team knows JS/TS)

| Layer      | Technology           | Why                                           |
| ---------- | -------------------- | --------------------------------------------- |
| Runtime    | Node.js 20+          | LTS, fast, huge ecosystem                     |
| Framework  | Fastify              | 2x faster than Express, schema-first, plugins |
| Language   | TypeScript           | Type safety                                   |
| Validation | Zod                  | Runtime + compile-time schema validation      |
| Database   | PostgreSQL + Drizzle | As above                                      |
| Testing    | Vitest + Supertest   | Fast, native ESM                              |
| Docs       | OpenAPI + Scalar     | Auto-generated, beautiful API docs            |

### Python (when team knows Python, or ML-adjacent)

| Layer      | Technology                          | Why                                      |
| ---------- | ----------------------------------- | ---------------------------------------- |
| Framework  | FastAPI                             | Async, auto OpenAPI, Pydantic validation |
| Language   | Python 3.11+                        | Type hints, async, fast                  |
| Validation | Pydantic v2                         | Fastest Python validation library        |
| Database   | PostgreSQL + SQLAlchemy or Tortoise | Mature, async-capable                    |
| Testing    | Pytest + HTTPX                      | Industry standard                        |

### Go (when performance is critical)

| Layer     | Technology             | Why                                           |
| --------- | ---------------------- | --------------------------------------------- |
| Framework | Fiber or Chi or stdlib | Fiber: Express-like; Chi: middleware-friendly |
| ORM       | GORM or sqlc           | sqlc: type-safe generated queries             |
| Testing   | Go testing + testify   | Built-in, fast                                |

**When to use Go:** High-throughput APIs (> 10K req/sec), microservices, infrastructure tools.

---

## Real-time / Collaborative Apps

**Recommended Stack: Next.js + WebSocket**

| Layer       | Technology                              | Why                                        |
| ----------- | --------------------------------------- | ------------------------------------------ |
| Frontend    | Next.js + React                         | Standard                                   |
| Real-time   | Liveblocks or Ably or Partykit          | Managed presence, conflict resolution      |
| Alternative | Socket.io (self-hosted)                 | More control, requires infra               |
| Database    | PostgreSQL + Supabase (Realtime)        | Built-in change events via Postgres        |
| State       | Y.js (for CRDT / collaborative editing) | Industry standard for conflict-free merges |

**When to use:** Figma-like tools, collaborative docs, live dashboards, multiplayer features.

---

## E-commerce

**Recommended Stack: Next.js + Commerce Layer**

| Layer             | Technology                                  | Why                                       |
| ----------------- | ------------------------------------------- | ----------------------------------------- |
| Frontend          | Next.js                                     | SEO critical for e-commerce               |
| Commerce Platform | Medusa.js (self-hosted) or Shopify Hydrogen | Medusa: full control; Shopify: proven     |
| Payment           | Stripe                                      | Best DX, global, subscriptions + one-time |
| Search            | Algolia or Typesense                        | Fast product search                       |
| Database          | PostgreSQL                                  | ACID for orders                           |

---

## AI-Powered Apps

**Recommended Stack: Next.js + Vercel AI SDK**

| Layer           | Technology                            | Why                                                  |
| --------------- | ------------------------------------- | ---------------------------------------------------- |
| Frontend        | Next.js                               | Streaming support, server components                 |
| AI SDK          | Vercel AI SDK                         | Provider-agnostic, streaming, tools/function calling |
| LLM Providers   | OpenAI / Anthropic / Gemini (via SDK) | Easy swap between providers                          |
| Vector Database | Pinecone or pgvector                  | pgvector: good enough for < 1M vectors, free         |
| Embeddings      | OpenAI text-embedding-3-small         | Cost-effective, high quality                         |
| RAG Framework   | LlamaIndex or LangChain               | Structure for complex pipelines                      |
| Caching         | Redis                                 | Cache LLM responses where appropriate                |

**Cost considerations:** Always calculate expected LLM call costs at scale. Add caching aggressively.

---

## Portfolio / Personal Brand

**Recommended Stack: Astro + MDX**

| Layer          | Technology                     | Why                                                     |
| -------------- | ------------------------------ | ------------------------------------------------------- |
| Framework      | Astro 4+                       | Static-first, zero JS by default, islands for interactivity |
| Content        | MDX + Content Collections      | Markdown with components, type-safe content queries     |
| Styling        | Tailwind CSS                   | Rapid styling, design-token driven                      |
| Fonts          | @fontsource / next/font        | Self-hosted, zero layout shift                          |
| Images         | Astro `<Image>` + AVIF         | Automatic optimization, responsive srcset               |
| Animations     | Framer Motion (islands)        | Scoped to interactive components only                   |
| Hosting        | Vercel / Cloudflare Pages      | Free tier, global CDN, instant deploys                  |
| Analytics      | Plausible / Umami              | Privacy-first, lightweight                              |
| CMS (optional) | Sanity / Decap CMS             | Non-technical editing for blog/portfolio content        |

**When to use:** Personal portfolios, brand sites, freelance showcases, creative resumes.

**Alternative:** Next.js with SSG — if you need React ecosystem or plan to add dynamic features later.

---

## Creative / Design Tool

**Recommended Stack: Next.js + Canvas/WebGL**

| Layer                | Technology                          | Why                                                  |
| -------------------- | ----------------------------------- | ---------------------------------------------------- |
| Frontend             | Next.js (App Router)                | SSR for landing, client-side for editor              |
| Canvas 2D            | Konva (react-konva) or Fabric.js    | Object-based canvas manipulation, hit detection      |
| WebGL / 3D           | Three.js via React Three Fiber      | Declarative 3D, great React integration              |
| Animation            | Framer Motion + GSAP                | UI transitions + timeline-based complex animations   |
| State                | Zustand + Immer                     | Lightweight, immutable updates for canvas state      |
| Input                | @use-gesture/react                  | Drag, pinch, scroll gestures for design interaction  |
| Persistence          | IndexedDB (via Dexie.js)            | Client-side storage for project files                |
| Export               | html2canvas / dom-to-image          | Rasterize designs to PNG/SVG                         |
| Backend              | Node.js + Fastify                   | File storage, collaboration, user accounts           |
| Real-time (optional) | Liveblocks / Y.js                   | Multi-user editing with CRDT conflict resolution     |

**When to use:** Design tools, whiteboard apps, image editors, creative coding platforms, prototyping tools.

**Alternative:** SvelteKit + svelte-canvas — smaller bundle, great for single-player creative tools.

---

## Gaming / Gamified Experience

**Recommended Stack: Next.js + Three.js / WebGL**

| Layer            | Technology                        | Why                                                |
| ---------------- | --------------------------------- | -------------------------------------------------- |
| Frontend         | Next.js                           | Landing pages, auth, leaderboards                  |
| 3D Engine        | Three.js + React Three Fiber (R3F) | Industry standard WebGL, huge ecosystem            |
| Physics          | @react-three/rapier or cannon-es  | Rapier: fast WASM physics; cannon-es: mature       |
| Game Loop        | Custom RAF loop or @react-three/drei | 60fps game loop with delta time                   |
| Audio            | Howler.js or Tone.js              | Howler: simple SFX; Tone.js: procedural/music      |
| State            | Zustand                           | Game state, inventory, player data                 |
| Shaders          | glsl-random / custom GLSL         | Custom visual effects, post-processing             |
| 2D Games         | Phaser.js or PixiJS               | Phaser: full game framework; PixiJS: lightweight renderer |
| Backend          | Node.js + WebSocket               | Multiplayer state, leaderboards, matchmaking       |
| Hosting          | Vercel (frontend) + Fly.io (game server) | Edge for UI, persistent for game state     |

**When to use:** Browser games, gamified onboarding, interactive storytelling, virtual worlds, 3D product configurators.

**Alternative:** Unity WebGL export — for complex 3D games with existing Unity expertise. Godot — open-source, exports to HTML5.

---

## Media & Content Platform

**Recommended Stack: Next.js + Headless CMS**

| Layer          | Technology                          | Why                                                 |
| -------------- | ----------------------------------- | --------------------------------------------------- |
| Frontend       | Next.js (App Router)                | SSR/SSG for SEO, fast page loads                    |
| CMS            | Sanity.io or Contentlayer           | Sanity: flexible schema, real-time; Contentlayer: local-first |
| Content Format | MDX                                 | Markdown + React components for rich editorial      |
| Typography     | Tailwind + custom CSS               | Editorial-grade type: drop caps, pull quotes, footnotes |
| Images         | Next/Image + Cloudinary             | Responsive, lazy-loaded, format-optimized           |
| Video          | Mux or Cloudflare Stream            | Adaptive bitrate, no buffering                      |
| Audio          | HTML5 Audio + custom player         | Podcast/music playback with waveform visualization  |
| Search         | Algolia or Pagefind                 | Full-text search across articles                    |
| Newsletter     | Resend + React Email                | Beautiful email templates, API-first                |
| Analytics      | PostHog or Plausible                | Track reading behavior, engagement                  |

**When to use:** Magazines, blogs, news sites, documentation platforms, content-heavy marketing sites, podcasts.

**Alternative:** Astro + MDX — if the site is mostly static with minimal interactivity. Ghost — self-hosted, built for publishing.

---

## Data Visualization / Dashboard Art

**Recommended Stack: Next.js + D3 / Observable**

| Layer             | Technology                        | Why                                                |
| ----------------- | --------------------------------- | -------------------------------------------------- |
| Frontend          | Next.js (App Router)              | SSR for initial render, client for interactivity   |
| Charting          | D3.js or Observable Plot          | D3: maximum control; Plot: declarative, D3-based   |
| Alternative Charts| Recharts or Nivo                  | Faster to build, less custom, React-native charts  |
| Animation         | Framer Motion + D3 transitions    | Smooth data transitions, animated axes             |
| Large Datasets    | WebGL via Deck.gl or regl         | GPU-accelerated rendering for 100K+ data points    |
| Maps              | Mapbox GL or deck.gl              | Vector tiles, 3D terrain, custom layers            |
| State             | TanStack Query + Zustand          | Fetch + cache data, manage filter/sort state       |
| Data Processing   | DuckDB-Wasm or Apache Arrow       | In-browser analytics on large datasets             |
| Export            | svg-crowbar / html-to-image       | Export charts as SVG/PNG for reports               |
| Backend           | Node.js + PostgreSQL              | Data API, aggregation queries                      |

**When to use:** Analytics dashboards, data storytelling, scientific visualization, financial dashboards, monitoring tools.

**Alternative:** SvelteKit + LayerCake — Svelte's reactivity model is excellent for data-driven visualizations.

---

## Event / Conference Website

**Recommended Stack: Astro + Content Collections**

| Layer          | Technology                        | Why                                                 |
| -------------- | --------------------------------- | --------------------------------------------------- |
| Framework      | Astro 4+                          | Static-first, fast, great for content-heavy sites   |
| Content        | Content Collections (MD/MDX)      | Type-safe speaker bios, schedules, session data     |
| Styling        | Tailwind CSS + custom animations  | Event branding, animated countdowns, hero sections  |
| Schedule UI    | Custom React island or Svelte     | Interactive schedule with filters, favorites        |
| Ticketing      | Stripe Payment Links or Eventbrite | External ticketing, no need to build from scratch   |
| Maps           | Mapbox or Leaflet                 | Venue maps, location directions                     |
| Countdown      | Framer Motion                     | Animated countdown to event start                   |
| Hosting        | Vercel / Cloudflare Pages         | Free, fast, handles traffic spikes on event day     |
| Email          | Resend + React Email              | Confirmation emails, speaker notifications          |
| Analytics      | Plausible                         | Track registrations, page views                     |

**When to use:** Conference sites, meetup pages, webinar landing pages, hackathon sites, product launch pages.

**Alternative:** Next.js — if you need dynamic features like live attendee dashboards or real-time Q&A.

---

## Developer Tool / CLI Companion

**Recommended Stack: Next.js + Code Highlighting**

| Layer            | Technology                        | Why                                                 |
| ---------------- | --------------------------------- | --------------------------------------------------- |
| Frontend         | Next.js (App Router)              | SSR for docs, client for interactive playgrounds    |
| Code Highlighting| Shiki or Prism.js                 | Shiki: VS Code-grade themes, accurate; Prism: lighter |
| Terminal UI      | xterm.js                          | Embedded terminal emulator for web-based CLIs       |
| Docs Framework   | Fumadocs or Nextra                | Purpose-built for developer documentation           |
| MDX              | contentlayer2 or fumadocs-mdx     | Interactive code blocks, embedded playgrounds       |
| Playground       | Sandpack (by CodeSandbox)         | In-browser code execution, live preview             |
| API Docs         | OpenAPI + Scalar or Stoplight     | Beautiful, interactive API reference                |
| CLI (companion)  | Commander.js or Yargs + Ink       | CLI tool with optional TUI (Ink for React-based)    |
| Styling          | Tailwind + shadcn/ui              | Clean, developer-friendly UI                        |
| Hosting          | Vercel (docs) + Railway (API)     | Docs on edge, API with persistent compute           |

**When to use:** Developer documentation sites, API explorers, CLI companion web apps, SDK playgrounds, interactive tutorials.

**Alternative:** Docusaurus — mature, plugin ecosystem, but heavier than Astro/Fumadocs for pure docs.

---

## Greenfield vs. Existing System Guidance

### Greenfield (Starting fresh)

- Prefer managed services over self-hosted — less ops overhead
- Use TypeScript for everything if JS ecosystem
- Pick Postgres — it does almost everything a startup needs
- Don't over-engineer — modular monolith scales further than people think

### Integrating with Legacy System

- Document all integration points as a risk register item
- Plan for schema mismatches — use an anti-corruption layer (adapter pattern)
- Consider whether to migrate or wrap the legacy API
- Define clear ownership boundaries

---

## Stack Decision Checklist

Before recommending a stack, verify:

- [ ] **Team familiarity:** What does the team already know? A known stack in the team is worth more than theoretically optimal.
- [ ] **Hosting budget:** Some stacks are expensive at scale (Vercel, managed DBs). Model the monthly cost at 10x current users.
- [ ] **Compliance requirements:** HIPAA → check if managed service has BAA. PCI → delegate card data to processor.
- [ ] **Timeline:** Tighter deadlines favor managed services (Supabase, Clerk, Resend) over self-hosted.
- [ ] **Scale projections:** Most startups over-engineer for scale. A Postgres + Node.js monolith handles millions of users with proper indexing.
- [ ] **Mobile requirement:** If mobile is critical, consider React Native from day one — retrofitting is painful.

---

## Common Anti-Patterns to Call Out in PRD

Flag these in the PRD's risk register if they appear:

1. **Premature microservices:** Almost always better to start with a monolith and extract services when a real bottleneck exists.
2. **Custom auth implementation:** Never roll your own auth — use a proven provider.
3. **No caching strategy:** Every API needs a cache layer design, even if not implemented day 1.
4. **Missing connection pooling:** PgBouncer or server-side pooling is essential with serverless.
5. **No database migration strategy:** "We'll just ALTER TABLE manually" is a disaster waiting to happen.
6. **Hard-coded configuration:** Secrets in code = security incident waiting to happen.
7. **No async jobs strategy:** Synchronous user-facing requests doing heavy work (email, PDF, AI) = bad UX and flaky APIs.

---

## Vibe-Specific Tech Additions

For vibe-driven products, these specialized libraries enable the sensory experience. Pick based on the aesthetic requirements defined in the Vibe PRD.

### Animation Engines

| Library | Bundle Size | Best For | Key Feature |
|---------|-------------|----------|-------------|
| **Framer Motion** | ~30KB | React UI animations | Declarative, layout animations, gestures, exit animations |
| **GSAP** | ~25KB (core) | Complex timelines, scroll-triggered | Industry standard for marketing sites, ScrollTrigger plugin |
| **Motion One** | ~5KB | Lightweight alternative to Framer | Smallest API surface, WAAPI-based, good for simple transitions |
| **Anime.js** | ~17KB | Vanilla JS projects | Framework-agnostic, SVG morphing, timeline control |
| **Lenis** | ~8KB | Smooth scrolling | Buttery scroll experience, works with any animation library |
| **React Spring** | ~18KB | Physics-based React animations | Spring physics, interruptible animations |

**Recommendation:** Framer Motion for React apps (default choice). GSAP for marketing/landing pages with complex scroll animations. Motion One when bundle size is critical.

### WebGL / 3D

| Library | Bundle Size | Best For | Key Feature |
|---------|-------------|----------|-------------|
| **Three.js** | ~150KB | Full 3D scenes, custom shaders | Industry standard, massive ecosystem, full control |
| **React Three Fiber (R3F)** | ~180KB (with Three) | React + Three.js | Declarative Three.js, React reconciliation, hooks |
| **Spline** | ~50KB | No-code 3D, quick prototypes | Visual editor, exports to React component |
| **OGL** | ~15KB | Minimal WebGL | Tiny footprint, modern WebGL2, functional approach |
| **Regl** | ~30KB | Data visualization, particle systems | Functional WebGL, great for 100K+ primitives |
| **Babylon.js** | ~500KB | Enterprise 3D, game-like experiences | Full engine: physics, PBR, post-processing built-in |

**Recommendation:** R3F for React apps needing 3D. Three.js for non-React or maximum control. Spline for quick visual experiments. OGL when bundle size matters.

### Shader & Visual Effects

| Library | Purpose | Notes |
|---------|---------|-------|
| **glsl-random** | Noise functions (Perlin, Simplex) | Essential for organic animations, clouds, terrain |
| **postprocessing** (three.js) | Bloom, chromatic aberration, depth of field | Post-processing pipeline for R3F/Three.js |
| **shader-park** | Procedural geometry, SDFs | Creative coding, generative art |
| **simplex-noise** | Vanilla JS noise | Framework-agnostic, good for canvas 2D effects |
| **glslify** | GLSL module system | Reusable shader code, npm ecosystem |

**When to use shaders:** Custom visual effects that can't be achieved with CSS alone — fluid simulations, particle systems, organic textures, real-time distortion.

### Audio

| Library | Bundle Size | Best For | Key Feature |
|---------|-------------|----------|-------------|
| **Howler.js** | ~10KB | Sound effects, simple audio | HTML5 Audio with Web Audio fallback, spatial audio |
| **Tone.js** | ~100KB | Procedural audio, music | Synthesizers, effects, sequencing, scheduling |
| **Web Audio API** | 0 (native) | Maximum control, custom DSP | Browser native, steep learning curve |
| **SoundJS** | ~30KB | Game audio | CreateJS suite, good for games |

**Recommendation:** Howler.js for UI sounds and SFX. Tone.js for generative/procedural audio or music apps. Web Audio API when you need custom processing.

### Canvas 2D

| Library | Bundle Size | Best For | Key Feature |
|---------|-------------|----------|-------------|
| **Konva (react-konva)** | ~50KB | Object-based canvas, React | Events, drag-drop, layer system, React bindings |
| **Fabric.js** | ~80KB | Image editing, object manipulation | Rich object model, SVG import/export |
| **Paper.js** | ~60KB | Vector graphics, computational design | Boolean operations, path simplification |
| **PixiJS** | ~100KB | High-performance 2D rendering | WebGL renderer with Canvas fallback, very fast |
| **P5.js** | ~100KB | Creative coding, education | Easy API, great for sketches and generative art |

**Recommendation:** react-konva for interactive diagrams/design tools. PixiJS for performance-critical 2D (games, visualizations). P5.js for creative coding and prototyping.

### Haptics & Advanced Input

| Library | Purpose | Notes |
|---------|---------|-------|
| **@use-gesture/react** | Drag, pinch, scroll, hover, move | Unified gesture API, works with any animation library |
| **react-spring** | Physics-based animations | Spring physics, interruptible, great with gestures |
| **Vibration API** (native) | Mobile haptic feedback | `navigator.vibrate()` — simple but limited |
| **Gamepad API** (native) | Controller input | For gamified experiences, browser-native |

**Recommendation:** @use-gesture for any interactive canvas or draggable UI. Combine with Framer Motion or react-spring for physics-based feedback.

### Choosing the Right Stack for Your Vibe

| Vibe Keywords | Recommended Combo |
|---------------|-------------------|
| "Elegant, minimal, refined" | Framer Motion + Lenis + subtle Howler SFX |
| "Playful, bouncy, fun" | Framer Motion + @use-gesture + Howler |
| "Immersive, cinematic, dramatic" | GSAP ScrollTrigger + Three.js + Tone.js ambient |
| "Futuristic, neon, cyberpunk" | Three.js + postprocessing (bloom) + custom shaders |
| "Organic, natural, flowing" | Three.js + simplex-noise + Lenis + generative audio |
| "Retro, pixel, nostalgic" | PixiJS + P5.js + Howler (chiptune SFX) |
| "Editorial, sophisticated" | Framer Motion + Lenis + custom typography animations |
