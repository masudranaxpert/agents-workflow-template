# Master Agent Skills Handbook & Decision Guide

> A production-grade directory and decision matrix for all 74 AI coding agent skills installed in the environment. Designed for instant lookup, architectural guidance, and selecting the optimal skill for any engineering task.

---

## ⚡ Quick Decision Matrix (Cheat Sheet)

| When You Want To... | Primary Skill | Supporting / Specialized Skill |
| :--- | :--- | :--- |
| **Design system architecture or decouple modules** | `codebase-design` | `api-and-interface-design` |
| **Build a fresh UI without generic AI aesthetics** | `frontend-design-complete` | `better-colors`, `better-typography` |
| **Engineer clean React / Tailwind components** | `frontend-ui-engineering` | `tailwind-4-docs`, `pick-ui-library` |
| **Build silky smooth web animations** | `animate` | `apple-design`, `emil-design-eng` |
| **Add fluid page transitions in Next.js / React** | `vercel-react-view-transitions` | `animate` |
| **Make a web app feel 100% native on mobile** | `mobile-native` | `animate-expo` (if React Native) |
| **Stress-test UI with realistic worst-case data** | `break-ui` | `break` (for visual isolation page) |
| **Generate multiple design variants to compare** | `variant` | `prototype` |
| **Optimize Next.js Core Web Vitals & Caching** | `nextjs-performance` | `vercel-react-best-practices` |
| **Implement RBAC / Auth in Next.js App Router** | `nextjs-authentication` | `nextjs-app-router-patterns` |
| **Build Django models, APIs and serializers** | `django-patterns` | `django-expert` |
| **Fix slow Django / ORM queries & N+1 bottlenecks** | `django-perf-review` | `performance-optimization` |
| **Build high-throughput async Python APIs** | `fastapi-patterns` | `fastapi-async-patterns`, `fastapi` |
| **Train ML models or fine-tune LLMs** | `ai-ml-development` | `ml-pipeline` |
| **Deploy & orchestrate MLOps pipelines** | `ml-pipeline` | `mle-workflow`, `deploying-machine-learning-models` |
| **Audit code security & detect vulnerabilities** | `security-audit` | `code-review-and-quality` |
| **Perform multi-axis code review before merge** | `code-review-and-quality` | `nextjs-code-review` / `react-doctor` |
| **Automate end-to-end browser tests** | `playwright-cli` | `browser-testing-with-devtools` |
| **Write an open-source README from scratch** | `crafting-effective-readmes` | `readme-optimization` (for audits) |
| **Remove chatbot / AI writing patterns from text** | `humanizer` | `no-ai-slop` (to keep author voice) |

---

## 🏛️ Domain 1: Architecture, Interfaces & Security

### `codebase-design`
- **When to Use:** When designing new features from scratch, restructuring sprawling folders, or refactoring tight coupling.
- **Key Focus:** Deep modules (small, simple interfaces hiding complex logic behind clean seams), adapters, and avoiding shallow abstractions.
- **Best Combined With:** `api-and-interface-design`, `code-review-and-quality`.

### `api-and-interface-design`
- **When to Use:** When designing public REST / GraphQL APIs, module seams, or shared TypeScript type definitions between frontend and backend.
- **Key Focus:** Stability, backwards compatibility, minimal breaking changes, and predictable error handling.

### `code-review-and-quality`
- **When to Use:** Before merging any PR or significant commit.
- **Key Focus:** Multi-axis code review (correctness, performance, security, maintainability), regression checks, and inverse mutation verification.

### `security-audit`
- **When to Use:** When auditing auth endpoints, role-based access control (RBAC), user input sanitization, API keys, or preparing for production deployment.
- **Key Focus:** Vulnerability detection, SQLi/XSS/CSRF prevention, secret leak detection, and security posture review.

---

## 🎨 Domain 2: Frontend Aesthetics & Visual Systems

### `frontend-design-complete`
- **When to Use:** When starting any web page or component where visual distinction matters. Use to prevent generic "AI slop" (cliché purple gradients on white backgrounds, standard card grids).
- **Key Focus:** Intentional aesthetics (brutalist, luxury, editorial, retro-future), OKLCH color palettes, bold layouts, and responsive design.

### `impeccable`
- **When to Use:** When polishing, distilling, or hardening an existing frontend interface that looks bland or cluttered.
- **Key Focus:** Visual hierarchy, cognitive load reduction, spacing rhythm, and high-craft polish.

### `better-colors`
- **When to Use:** Setting up a project's color palette, switching to OKLCH, defining semantic tokens (`--surface`, `--accent`), or ensuring WCAG contrast compliance.

### `better-typography`
- **When to Use:** Defining type scales, font pairings (display vs body), line heights, variable font settings, and handling text truncation/overflow.

### `better-layout`
- **When to Use:** Responsive grid systems, optical alignment, spacing consistency, and ensuring layouts hold up across multiple screen widths.

### `better-ui`
- **When to Use:** Polishing physical interface details: concentric border radii (`outer = inner + padding`), shadow rings instead of harsh borders, optical icon offsets.

### `better-writing`
- **When to Use:** Writing or auditing UI microcopy: clear button labels, actionable error messages, helpful empty states, and toast notifications.

### `better-accessibility`
- **When to Use:** Auditing against WCAG 2.2 AA/AAA: keyboard navigation, focus rings (`:focus-visible`), ARIA attributes, tap targets (minimum 44x44px).

### `better-interface`
- **When to Use:** Running a single comprehensive review combining all `better-*` dimensions (layout, color, type, writing, a11y, polish) in one pass.

### `build-design`
- **When to Use:** When converting Figma screenshots or UI mockups into pixel-accurate code using your existing project tokens.

---

## 🧩 Domain 3: Component Engineering & Frameworks

### `frontend-ui-engineering`
- **When to Use:** Writing production-grade React components.
- **Key Focus:** Composition over configuration, component colocation, accessible form handling, and resilient state machines.

### `frontend-patterns`
- **When to Use:** Structuring React / Next.js component state, preventing unnecessary re-renders, and organizing component trees.

### `tailwind-4-docs`
- **When to Use:** Working with Tailwind CSS v4.
- **Key Focus:** CSS-first `@theme` configuration, modern utility classes, container queries, and migrating from Tailwind v3.

### `pick-ui-library`
- **When to Use:** Deciding which third-party component library or headless primitive fits your stack best (shadcn/ui, Radix, Base UI, Ark UI, etc.).

### `react`
- **When to Use:** Working with `@json-render/react` or converting JSON specifications into dynamic React interfaces.

### `react-components`
- **When to Use:** Converting Stitch designs into modular Vite/React components or synchronizing React code with Stitch canvas.

### `react-doctor`
- **When to Use:** Running diagnostics on React codebases to identify hook violations, state mutations, accessibility failures, and performance leaks.

### `htmx`
- **When to Use:** Building dynamic, interactive UIs driven by server HTML swaps without the overhead of client-side JavaScript frameworks.

### `alpine-js`
- **When to Use:** Adding lightweight reactive micro-interactions (dropdowns, modals, toggles) to server-rendered templates (Laravel Blade, Django, HTML).

---

## 🎬 Domain 4: Motion, Animations & Apple-Grade Craft

### `animate`
- **When to Use:** Building any web animation from scratch.
- **Key Focus:** Deciding whether to animate, spring physics vs cubic-bezier easing, exit animations, and interruptible gesture transitions.

### `emil-design-eng`
- **When to Use:** Injecting high-craft micro-interactions into buttons, cards, popovers, and inputs.
- **Key Focus:** Emil Kowalski's philosophy: invisible details, delight without delay, tactile feedback.

### `apple-design`
- **When to Use:** Creating Apple-inspired interfaces: translucent materials (`backdrop-filter`), fluid momentum gestures, spring-driven bottom sheets.

### `animate-expo`
- **When to Use:** Building mobile animations in React Native / Expo using Reanimated, Gesture Handler, and haptics.

### `animation-vocabulary`
- **When to Use:** When you have a motion effect in mind but don't know the exact technical term ("Rubber-banding", "Pop in", "Shared element transition").

### `find-animation-opportunities`
- **When to Use:** Scanning an existing static codebase to identify places where subtle motion would elevate the experience.

### `review-animations`
- **When to Use:** Reviewing animation code against performance best practices (compositor thread, `transform`/`opacity` only, reduced motion support).

### `improve-animations`
- **When to Use:** Creating a prioritized refactoring roadmap for an entire application's motion architecture.

### `ask-sonner`
- **When to Use:** Adding toasts and notification feeds using the Sonner React library (promise toasts, custom layouts, theme syncing).

### `vercel-react-view-transitions`
- **When to Use:** Implementing native-feeling page navigation and shared element transitions in Next.js / React using the View Transitions API.

---

## 🧪 Domain 5: UI Variations, Prototyping & Stress-Testing

### `break-ui` (Emil Kowalski)
- **When to Use:** In-place adversarial data stress-testing. Injects realistic worst-case data (extreme names, zero items, unbreakable emails) behind a toggle.

### `break` (Jakub Krehel)
- **When to Use:** Isolated scenario testing. Generates a dedicated temporary test page to display every component variant and state side-by-side.

### `variant`
- **When to Use:** When designing a component and you want to generate 3–4 distinct visual variations to pick the best one.

### `prototype`
- **When to Use:** Rapidly building multiple divergent implementations of a user interface concept from scratch.

### `state-machine`
- **When to Use:** Rendering every discrete lifecycle state (loading, error, empty, success, editing) of a complex component with a visual switcher.

### `explain-interface`
- **When to Use:** Reverse-engineering how an impressive web effect or interactive UI was built from a URL or screenshot.

---

## ⚡ Domain 6: Next.js & Full-Stack React

### `nextjs-developer`
- **When to Use:** Building Next.js App Router applications: Server Actions, parallel routes, route handlers, and streaming SSR.

### `nextjs-app-router-patterns`
- **When to Use:** Deep App Router architectural patterns: Server Components vs Client Components boundaries and optimized data fetching.

### `nextjs-authentication`
- **When to Use:** Implementing authentication in Next.js 15+ using Auth.js v5 (NextAuth), OAuth providers, database adapters, and protected route middleware.

### `nextjs-performance`
- **When to Use:** Optimizing Next.js for Core Web Vitals (LCP, INP, CLS), `next/image`, font preloading, streaming Suspense, and advanced caching (`revalidateTag`).

### `nextjs-code-review`
- **When to Use:** Auditing Next.js code before shipping to verify server boundary safety, data leak prevention, and cache efficiency.

### `vercel-react-best-practices`
- **When to Use:** Applying Vercel Engineering's 70 performance rules: eliminating barrel file overhead, dynamic imports, and bundle minimization.

---

## 🐍 Domain 7: Backend Engineering: Python & Django

### `django-patterns`
- **When to Use:** Building end-to-end Django architectures, REST APIs with DRF, modular applications, and clean service layers.

### `django-expert`
- **When to Use:** Specialized reference guides for DRF serializers, viewsets, authentication backends, and Django test cases.

### `django-perf-review`
- **When to Use:** Auditing Django database queries to eliminate N+1 bottlenecks, optimize `select_related`/`prefetch_related`, and configure DB indexes.

### `python-design-patterns`
- **When to Use:** Applying SOLID, KISS, and composition-over-inheritance patterns to Python services and data models.

### `python-performance-optimization`
- **When to Use:** Profiling slow Python code with `cProfile`, finding memory leaks, and optimizing CPU-bound algorithms.

---

## 🚀 Domain 8: Backend Engineering: FastAPI

### `fastapi`
- **When to Use:** General FastAPI API development, Pydantic model validation, dependency injection (`Depends`), and SSE/Streaming endpoints.

### `fastapi-patterns`
- **When to Use:** Structuring production-ready FastAPI applications with clean service repositories, transactional layers, and pytest fixtures.

### `fastapi-async-patterns`
- **When to Use:** High-concurrency async patterns: non-blocking database pools (asyncpg/SQLAlchemy 2 async), asyncio task groups, and background tasks.

---

## 🐹 Domain 9: Systems & Native: Go & Swift

### `golang-design-patterns`
- **When to Use:** Idiomatic Go design: functional options pattern, constructor APIs, error wrapping (`errors.Is`/`As`), and graceful shutdown routines.

### `golang-popular-libraries`
- **When to Use:** Selecting vetted, production-grade Go libraries for routing, database access, logging, and metrics.

### `golang-documentation`
- **When to Use:** Writing idiomatic Godoc comments, example tests, and developer documentation for Go packages and CLI tools.

### `write-swift`
- **When to Use:** Writing modern Swift 6 code: value types, Actor concurrency, data-race safety, ARC memory management, and Swift Testing.

---

## 🤖 Domain 10: AI, Machine Learning & MLOps

### `ai-ml-development`
- **When to Use:** Developing ML models with PyTorch or TensorFlow, training loops, and LLM fine-tuning pipelines.

### `ml-pipeline`
- **When to Use:** Setting up MLOps infrastructure: orchestrating DAGs with Airflow / Kubeflow, experiment tracking with MLflow / W&B, and feature stores with Feast.

### `mle-workflow`
- **When to Use:** Production machine learning workflows: strict data contracts, reproducible validation, drift monitoring, and rollback strategies.

### `deploying-machine-learning-models`
- **When to Use:** Packaging and serving ML models in production (Triton, FastAPI, ONNX Runtime) with low latency.

---

## 🔍 Domain 11: Testing, QA & DevTools

### `browser-testing-with-devtools`
- **When to Use:** Testing live web applications directly inside a headless or headed Chrome instance via Chrome DevTools MCP.

### `chrome-devtools-mcp`
- **When to Use:** Inspecting live DOM trees, CSS computed styles, monitoring network requests, and capturing runtime console errors.

### `playwright-cli`
- **When to Use:** End-to-end automated UI testing, running headless browser scripts, and filling forms across multiple viewports.

### `performance-optimization`
- **When to Use:** Cross-stack profiling to identify bottlenecks across frontend rendering, API latency, and database query times.

---

## 📝 Domain 12: Documentation & Prose Engineering

### `crafting-effective-readmes`
- **When to Use:** Writing a new README from scratch for any project (CLI tool, open-source library, SaaS web app).

### `readme-optimization`
- **When to Use:** Auditing and rewriting an existing README to maximize developer conversion, reduce friction, and verify quickstart instructions.

### `no-ai-slop`
- **When to Use:** Editing technical blogs, drafts, or documentation to sharpen clarity while strictly preserving the author's personal voice.

### `humanizer`
- **When to Use:** Scrubbing corporate AI-generated prose using Wikipedia's 20 signs of AI writing (removing forced triads, staging, and inflated claims).

---

## 📱 Domain 13: Mobile-Native & Cloud Operations

### `mobile-native`
- **When to Use:** Making web apps feel indistinguishable from installed mobile apps (notch spacing, 100vh viewport fixes, zero tap delay, disabling sticky hover).

### `nextdeploy-cli`
- **When to Use:** Deploying and managing applications using the NextDeploy CLI (`nd push`, container management, environment sync).

### `nextdeploy-mcp`
- **When to Use:** Automating NextDeploy operations directly via Model Context Protocol tools.

### `api-recon-and-docs`
- **When to Use:** Discovering undocumented API endpoints, mapping Swagger / OpenAPI schemas, and analyzing API surface areas.

---

## 🏗️ Real-World Scenario Blueprints

### Blueprint 1: Building an E-Commerce CRM
1. **Architecture & Seams:** `codebase-design` (isolate Order, Customer, and Refund logic into deep modules).
2. **Backend & Queries:** `django-patterns` + `django-perf-review` (or `fastapi-patterns` + `fastapi-async-patterns`).
3. **Admin Dashboard UI:** `frontend-design-complete` (clean theme) + `frontend-ui-engineering` (accessible data tables).
4. **Micro-Interactions & Alerts:** `better-ui` + `ask-sonner` (instant toast notifications).
5. **Stress-Testing:** `break-ui` (test with extreme customer names, long emails, zero-order states).
6. **Security & Code Review:** `security-audit` + `code-review-and-quality`.

### Blueprint 2: High-Converting SaaS Landing Page
1. **Art Direction & Theme:** `frontend-design-complete` + `better-typography` + `better-colors`.
2. **Interactive Motion:** `animate` (staggered hero reveal) + `apple-design` (glassmorphic feature cards).
3. **Mobile Polish:** `mobile-native` (ensure no tap delays or horizontal overflow on iOS/Android).
4. **Copy Polish:** `better-writing` + `no-ai-slop` (direct, human value propositions).
5. **Performance Audit:** `nextjs-performance` (100 Lighthouse score on Core Web Vitals).

### Blueprint 3: High-Throughput Microservice API
1. **Framework & Engine:** `fastapi` + `fastapi-async-patterns` (or `golang-design-patterns`).
2. **API Contract:** `api-and-interface-design` (type-safe Pydantic / Go schemas).
3. **Resilience & Testing:** `performance-optimization` + `code-review-and-quality` (mutation tests).
4. **Documentation:** `crafting-effective-readmes` + `golang-documentation`.
