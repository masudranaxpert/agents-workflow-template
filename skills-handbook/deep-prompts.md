# Deep Prompting & Agent Audit Guide

A complete guide to eliminating AI sycophancy, triggering exhaustive deep thinking, and running rigorous code audits using battle-tested prompt engineering patterns and Antigravity slash commands.

---

## 1. The Sycophancy Problem: Why AI Agents Skim

এআই মডেলগুলোকে যখন সাধারণ ভাষায় বলা হয় *"কোডটা একটু দেখো"* বা *"Review this UI"*, তখন মডেলটি **Sycophancy (ব্যবহারকারীকে খুশি করার প্রবণতা)** এবং **Superficial Skimming** মোডে চলে যায়।

### কেন এমন হয়?
- **RLHF Bias:** মডেলগুলোকে ট্রেইনিংয়ের সময় বিনয়ী, একমত হওয়া এবং পজিটিভ উত্তর দেওয়ার জন্য রিওয়ার্ড দেওয়া হয়েছে। ফলে ডিফল্ট অবস্থায় তারা কঠোর সমালোচনা না করে বলে *"Everything looks great!"*
- **Token Laziness (গড়ের ফাঁদ):** বড় কোডবেস স্ক্যান করার সময় এআই প্রথম ২-১টি ফাইল চোখ বুলিয়ে সিদ্ধান্ত নিয়ে ফেলে (স্যাম্পলিং করে), পুরো ডেটা-ফ্লো বা রেন্ডারিং সাইকেল ট্রেস করে না।

এই অলসতা ও ফাঁকিবাজি ভাঙার একমাত্র উপায় হলো প্রম্পটে **কঠোর মনস্তাত্ত্বিক বাধা (Psychological Constraints)** এবং **লেন্সভিত্তিক স্ট্রাকচার** দেওয়া।

---

## 2. Six Rules for Exhaustive Deep Thinking

রেডিট (r/ChatGPTCoding, r/ClaudeAI), এক্স এবং টপ এআই ইঞ্জিনিয়ারদের পরীক্ষিত ৬টি মূলনীতি:

### Rule 1: Kill Flattery (প্রশংসা সম্পূর্ণ নিষিদ্ধ করুন)
- **কৌশল:** এআই-কে শুরুতেই জানিয়ে দিন যে মিষ্টি কথা বলা বা প্রশংসা করা শাস্তিযোগ্য।
- **ট্রিগার ফ্রেজ:**  
  `"Be brutally honest. Zero flattery. Do not praise the code. Your only job is to find flaws, fragility, and technical debt."`

### Rule 2: Force Line-by-Line Execution Tracing (স্যাম্পলিং বন্ধ করুন)
- **কৌশল:** "Review" শব্দের বদলে "Execution Trace" শব্দ ব্যবহার করুন।
- **ট্রিগার ফ্রেজ:**  
  `"Perform an exhaustive line-by-line audit. Do not skim or summarize. Walk through the execution path from input trigger to final render."`

### Rule 3: Adversarial Persona (শত্রুভাবাপন্ন টেস্টার বানান)
- **কৌশল:** এআইকে একজন হেল্পফুল অ্যাসিস্ট্যান্ট না বানিয়ে প্রোডাকশন ভাঙতে চাওয়া টেস্টার বানান।
- **ট্রিগার ফ্রেজ:**  
  `"Act as an adversarial Principal QA Architect trying to break this application in production under worst-case real-world conditions."`

### Rule 4: Multi-Lens Separation (দৃষ্টিভঙ্গি ভাগ করে দিন)
- **কৌশল:** এআইকে একবারে ঢালাওভাবে ভাবতে না দিয়ে ৪–৫টি আলাদা ক্যাটাগরি বা লেন্স ধরিয়ে দিন। এতে প্রতিটির গভীরে ভাবতে বাধ্য হয়।

### Rule 5: Evidence-Based Verification (প্রমাণ ছাড়া কথা বন্ধ)
- **কৌশল:** সাধারণ অনুমানের বদলে ফাইলের নাম, লাইন নম্বর এবং রুট-কজ বাধ্যতামূলক করুন।
- **ট্রিগার ফ্রেজ:**  
  `"For every issue found, provide: [Severity] | [File:Line] | [Failure Mode] | [Root Cause] | [Code Fix]. If no issue exists in a category, explicitly state 'No concerns found' instead of generic filler text."`

### Rule 6: Assume Broken Until Proven Otherwise
- **কৌশল:**  
  `"Assume this implementation has at least three critical edge-case bugs until proven otherwise."`

---

## 3. Antigravity Built-in Slash Commands Reference

আমাদের সিস্টেমে ডিপ থিংকিং ও স্বয়ংক্রিয় গবেষণার জন্য কিছু শক্তিশালী বিল্ট-ইন স্ল্যাশ কমান্ড রয়েছে। সাধারণ প্রম্পটের শুরুতে এগুলো যুক্ত করলে এজেন্টের পাওয়ার বহুগুণ বেড়ে যায়:

| Slash Command | কী কাজ করে | কখন ব্যবহার করবেন |
| :--- | :--- | :--- |
| **`/boost`** | মডেলকে মাল্টি-অ্যাঙ্গেল ডিপ থিংকিং, স্ট্র্যাটেজিক প্ল্যানিং এবং রিগোরাস ভেরিফিকেশন মোডে পাঠায়। | যখন জটিল কোডবেস অডিট, বড় রিফ্যাক্টরিং বা ডিপ স্ক্যান দরকার। |
| **`/grill-me`** | এজেন্ট নিজে ইন্টারঅ্যাক্টিভ ইন্টারভিউ নিয়ে আপনার কাছ থেকে প্রতিটি ডিজাইন ও এজ-কেস রিকোয়ারমেন্টস পরিষ্কার করে নেবে। | কোনো ফিচার শুরু করার আগে যখন রিকোয়ারমেন্টস অস্পষ্ট বা ফাঁক থাকে। |
| **`/goal`** | অটোনোমাস রিলেন্টলেস মোড। টাস্কের শতভাগ লক্ষ্য অর্জিত না হওয়া পর্যন্ত ব্যাকগ্রাউন্ডে থামবে না। | ওভারনাইট বা লং-রানিং বড় প্রজেক্ট স্বয়ংক্রিয়ভাবে শেষ করতে। |
| **`/plan`** | কোডে হাত দেওয়ার আগে ধাপে ধাপে আর্কিটেকচারাল প্ল্যান তৈরি করবে এবং অনুমোদন চাইবে। | জটিল ফিচার যেখানে আগেভাগে প্ল্যানিং জরুরি। |
| **`/browser`** | সরাসরি লাইভ ব্রাউজার অটোমেশন, ওয়েব পেজ ইন্টারঅ্যাকশন ও ডম ইন্সপেকশন চালাবে। | যখন UI ক্লিক, ফর্ম টেস্ট বা লাইভ ওয়েব ডিবাগিং দরকার। |
| **`/learn`** | ইউজারের দেওয়া কারেকশন বা স্পেশাল নিয়মগুলো মেমোরিতে সেভ করে রাখবে ভবিষ্যতের জন্য। | যখন এজেন্টকে কোনো স্থায়ী নিয়ম শেখাতে চান। |
| **`/schedule`** | নির্দিষ্ট সময় পরপর বা এককালীন ব্যাকগ্রাউন্ড টাইমার দিয়ে টাস্ক চালাবে। | পিরিয়ডিক হেলথ চেক বা শিডিউলড অটোমেশনের জন্য। |

---

## 4. Ready-to-Use Master Prompts

### Prompt 1: Adversarial UI & Layout Deep Scan

```text
/boost
Act as an adversarial Principal Design Director and QA Architect. Perform an exhaustive line-by-line audit of this UI codebase.

Rules:
1. Be brutally honest. Zero flattery. Do not praise anything.
2. Assume the layout will break in production until proven otherwise.
3. Trace the actual rendering flow and evaluate through these 5 strict lenses:
   - Stacking & Layering: (Z-index collisions, dropdown clipping, modals behind cards, sticky nav overlap)
   - Layout Fragility: (Overflow clipping, long unbreakable text, 0 items, 1 item, empty states)
   - Color & Contrast: (WCAG AA/AAA contrast failure, generic AI-slop purple gradients, unstyled tokens)
   - Mobile Native Feel: (Horizontal scrollbars, tap targets < 44px, iOS notch cutoffs, 100vh bugs)
   - Micro-Interactions: (Missing active/focus-visible states, jarring un-eased transitions)

Output format:
Provide findings in a table:
| Severity (Critical/High/Medium) | Component / File:Line | What Breaks in Production | Root Cause | Exact CSS/Code Fix |

If an area has no issues, explicitly write "No concerns found" instead of generic praise.
```

---

### Prompt 2: Backend Architecture & Security Deep Scan

```text
/boost
You are a Principal Software Architect and AppSec Lead conducting an exhaustive production-readiness audit. Your goal is not to explain the code, but to uncover hidden risks, technical debt, and architectural failure modes.

Analyze this codebase through these 6 lenses:
1. Security: Injection risks, auth/RBAC bypass, exposed sensitive fields, missing input validation.
2. Database Efficiency: N+1 query patterns, missing indexes on filter/sort fields, transaction boundaries.
3. Concurrency & Async: Event loop blocking, race conditions, connection pool exhaustion.
4. Error Handling: Silent exception swallowing, non-standard error responses (RFC 7807 compliance).
5. Code Health: High cyclomatic complexity, tight coupling, leaky abstractions.
6. API Design: Idempotency failures, missing pagination limits.

Instructions:
- Be brutally skeptical. Do not compliment the author.
- Cite exact file paths and line numbers for every finding.
- Conclude with a prioritized top-3 action items list.
```

---

### Prompt 3: Interactive Visual Color Studio Generator

```text
Act as a Principal Design Systems Architect.
I am building: "[INSERT_PROJECT_NAME_OR_DESCRIPTION, e.g., A minimalist specialty coffee e-commerce / A high-density DevOps monitoring dashboard]".

I cannot judge colors from raw hex codes or text descriptions alone. Do NOT just output markdown text with color tables.

Instead, construct a single self-contained interactive HTML preview file named "palette-studio.html".

Requirements for the interactive HTML file:
1. Curated Theme Baseline: Provide multiple distinct curated theme presets (e.g. Linear High-Tech, Modern Platform, Hyperion Mint, Warm Craft, Nordic Forest) with live Dark and Light mode toggles.
2. Custom Color Fine-Tuning (Mandatory):
   - Every color token card (--color-bg, --color-surface, --color-text, --color-muted, --color-accent) MUST have an interactive native color picker (<input type="color">) and an editable hex text input.
   - The user must be able to click any swatch or type any custom hex to customize accents, backgrounds, or surfaces on the fly.
3. Realtime Component & Math Recalculation:
   - When any color is picked or modified, immediately update the live component preview (Hero banner, CTA buttons, metrics cards, status pills).
   - Recalculate WCAG contrast ratios in real time using relative luminance math and update the AAA/AA contrast badges dynamically.
4. Export: Provide a 1-click "Copy CSS Variables" button that copies the currently active (or customized) tokens formatted for :root and dark mode.
5. Zero dependencies: pure semantic HTML, vanilla CSS variables, and lightweight JS.
```

---

### Prompt 4: Pre-Merge Regression Gate

```text
Act as a skeptical Release Engineer reviewing this proposed pull request/diff.

Verification steps:
1. Mutation Check: If I invert one conditional logic check (flip === to !== or swap && to ||), would our existing test suite catch it?
2. Breaking Changes: Does this change any public API contract, prop interface, or database column without a migration?
3. State Leaks: Are there any useEffect memory leaks, dangling subscriptions, or unhandled promise rejections?

Give me a simple PASS or FAIL recommendation with bulleted evidence.
```

---

### Prompt 5: Elite UI Meta-Prompt Generator

```text
Act as a Principal Design Architect & Prompt Engineer. 
I want to build: "[INSERT_RAW_IDEA_HERE, e.g., A minimalist specialty coffee beans e-commerce / A high-density CRM for freelance engineers / A podcast discovery web app]".

Do not write the code yet. Instead, generate a comprehensive, bulletproof, anti-AI-slop design specification prompt that I can feed into an AI coding agent to get a world-class UI.

The generated prompt MUST structure the requirements across:
1. Exact Persona & Target Audience (preventing generic corporate templates)
2. Aesthetic Anchor & Vibe (choosing from Linear Dark, Vercel Clean, Teenage Engineering Industrial, Stripe Dense, or Warm Editorial Craft)
3. 60-30-10 Color System (exact Hex tokens for Base, Surface, Text, and ONE High-Impact Accent)
4. Typographic Hierarchy (exact Google font pairing with weights)
5. Layout Anatomy & Sections (concrete, interactive components with real purpose)
6. Banned Anti-Slop Constraints (explicitly prohibiting generic purple gradients, fake cards, floaty glassmorphism, or placeholder lorem ipsum)

Output ONLY the ready-to-copy execution prompt inside a clean markdown codeblock.
```

