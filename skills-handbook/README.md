# Master Skills Handbook

A structured directory and decision matrix for all 74 AI coding agent skills installed in the environment.

For a dedicated deep dive into UI, design systems, and motion, see **[UI Skills Handbook](ui.md)**.

---

## Quick Decision Matrix

| Task / Domain | Primary Skill | Supporting / Specialized Skill |
| :--- | :--- | :--- |
| **System Architecture & Module Boundaries** | `codebase-design` | `api-and-interface-design` |
| **UI Design without AI Slop** | `frontend-design-complete` | `better-colors`, `better-typography` |
| **Production React & Tailwind Components** | `frontend-ui-engineering` | `tailwind-4-docs`, `pick-ui-library` |
| **Web Animations from Scratch** | `animate` | `apple-design`, `emil-design-eng` |
| **Next.js Page Transitions & Shared Elements** | `vercel-react-view-transitions` | `animate` |
| **Native Feel on Mobile Web Apps** | `mobile-native` | `animate-expo` (React Native) |
| **UI Stress-Testing with Worst-Case Data** | `break-ui` | `break` (Visual isolation page) |
| **Design Variations & Comparison** | `variant` | `prototype` |
| **Next.js Core Web Vitals & Caching** | `nextjs-performance` | `vercel-react-best-practices` |
| **Next.js Authentication & RBAC** | `nextjs-authentication` | `nextjs-app-router-patterns` |
| **Django Backend Models, Views & APIs** | `django-patterns` | `django-expert` |
| **Django Database Queries & N+1 Fixes** | `django-perf-review` | `performance-optimization` |
| **High-Throughput Async FastAPI APIs** | `fastapi-patterns` | `fastapi-async-patterns`, `fastapi` |
| **ML Model Training & LLM Fine-Tuning** | `ai-ml-development` | `ml-pipeline` |
| **MLOps Pipeline & Model Serving** | `ml-pipeline` | `mle-workflow`, `deploying-machine-learning-models` |
| **Code Security & Bug Checking** | `security-audit` | `code-review-and-quality` |
| **Pre-Merge Regression & Code Review** | `code-review-and-quality` | `nextjs-code-review` / `react-doctor` |
| **End-to-End Automated Browser Testing** | `playwright-cli` | `browser-testing-with-devtools` |
| **Writing Open-Source READMEs** | `crafting-effective-readmes` | `readme-optimization` (for audits) |
| **Scrubbing AI Writing Tells** | `humanizer` | `no-ai-slop` (to keep author voice) |

---

## 1. Architecture, Interfaces & Security

- **`codebase-design`**: বড় ফিচার শুরুর আগে Deep Module আর্কিটেকচার তৈরি করতে (জটিল বিজনেস লজিক ছোট ও স্পষ্ট Interface-এর পেছনে রাখা)।
- **`api-and-interface-design`**: Frontend ও Backend-এর মধ্যে অপরিবর্তনশীল ও পরিষ্কার REST / GraphQL Type Contract তৈরি করতে।
- **`code-review-and-quality`**: যেকোনো কোড মার্জ করার আগে Regression ও Mutation Testing দিয়ে কোয়ালিটি ভেরিফাই করতে।
- **`security-audit`**: Authentication, RBAC Permissions, SQL Injection, XSS এবং Secret Leak স্ক্যান করতে।

---

## 2. Frontend Design, UI & Motion

> বিস্তারিত গাইডলাইন, লেআউট গাইড এবং Impeccable কমান্ডগুলোর জন্য পড়ুন: **[UI Skills Handbook](ui.md)**

- **`frontend-design-complete`**: জেনেরিক ChatGPT স্টাইলের সাদামাটা "AI-slop" ডিজাইন এড়িয়ে প্রফেশনাল, ইউনিক আর্ট ডিরেকশন তৈরি করতে।
- **`impeccable`**: পুরো UI-এর ভিজ্যুয়াল হায়ারার্কি, ব্যালেন্স এবং ফিনিশিং ক্রাফট টপ-কোম্পানির ডিজাইনারদের মানে নিয়ে যেতে।
- **`frontend-ui-engineering`**: ক্লিন React কোড আর্কিটেকচার—Composition over configuration, কাস্টম হুক ও ফর্ম স্টেট হ্যান্ডলিং।
- **`tailwind-4-docs`**: Tailwind CSS v4-এর আধুনিক `@theme` কনফিগারেশন ও নতুন CSS-first ইউটিলিটি ব্যবহার করতে।
- **`animate`**: স্ক্র্যাচ থেকে ওয়েব অ্যানিমেশন তৈরি—Spring Physics, Cubic-bezier Easing এবং এন্ট্রি/এক্সিট ট্রানজিশন বানাতে।
- **`apple-design`**: অ্যাপল স্টাইলের ফ্লুইড জেসচার, Translucent Glass Materials (`backdrop-filter`) এবং মোমেন্টাম স্প্রিং বটম-শিট বানাতে।
- **`ask-sonner`**: চমৎকার ও রেসপন্সিভ Sonner Toast নোটিফিকেশন যুক্ত করতে।
- **`break-ui`**: বাস্তবজীবনের চরম বাজে ডেটা দিয়ে ইন-প্লেস স্ট্রেস-টেস্ট করতে।
- **`break`**: আলাদা টেস্ট পেজ বানিয়ে কম্পোনেন্টের সব ভিজ্যুয়াল স্টেট পাশাপাশি দেখতে।
- **`variant`**: একই কম্পোনেন্টের ৩–৪টি ভিন্ন ডিজাইন ভ্যারিয়েশন তৈরি করে তুলনা করতে।

---

## 3. Next.js & Full-Stack React

- **`nextjs-developer`**: App Router ফিচার—Server Actions, Parallel Routes, রুট হ্যান্ডলার এবং স্ট্রিমিং SSR কোডিংয়ে।
- **`nextjs-app-router-patterns`**: Server Components ও Client Components বাউন্ডারি নিখুঁতভাবে আলাদা করতে এবং ডেটা ফেচিং আর্কিটেকচারে।
- **`nextjs-authentication`**: Auth.js v5 (NextAuth), ডেটাবেস এডাপ্টার, OAuth লগইন এবং রোল-বেসড সিকিউরিটি মিডলওয়্যার সেট করতে।
- **`nextjs-performance`**: Core Web Vitals (LCP, INP, CLS) ১০০ করতে, ইমেজ/ফন্ট অপটিমাইজেশন এবং `revalidateTag` দিয়ে অ্যাডভান্সড ক্যাশিংয়ে।
- **`nextjs-code-review`**: Next.js কোডবেসে সার্ভার সাইড সিকিউরিটি লিক, বাউন্ডারি ভুল বা ক্যাশ প্রবলেম অডিট করতে।
- **`vercel-react-best-practices`**: Vercel Engineering-এর ৭০টি পারফরম্যান্স রুলস মেনে বান্ডেল সাইজ কমাতে ও ডায়নামিক ইম্পোর্ট করতে।

---

## 4. Backend Engineering: Python & Django

- **`django-patterns`**: পরিচ্ছন্ন Django আর্কিটেকচার, সার্ভিস লেয়ার, মডুলার অ্যাপ স্ট্রাকচার এবং DRF REST API তৈরিতে।
- **`django-expert`**: DRF Serializers, ViewSets, কাস্টম ম্যানেজার এবং Django টেস্ট কেস দ্রুত রেফারেন্স করতে।
- **`django-perf-review`**: Sentry-র গাইডলাইনে ডেটাবেস অডিট করতে—`N+1` কুয়েরি দূর করা, `select_related`/`prefetch_related` ঠিক করা এবং ইনডেক্সিংয়ে।
- **`python-design-patterns`**: পাইথনে অবজেক্ট ও ফাংশনাল ডিজাইন প্যাটার্ন (KISS, SOLID, Composition) সঠিকভাবে প্রয়োগ করতে।
- **`python-performance-optimization`**: পাইথনের ধীর গতির ফাংশন `cProfile` দিয়ে মেপে বটলনেক এবং মেমোরি লিক ফিক্স করতে।

---

## 5. Backend Engineering: FastAPI

- **`fastapi`**: সাধারণ FastAPI এন্ডপয়েন্ট, Pydantic ভ্যালিডেশন, ডিপেনডেন্সি ইনজেকশন (`Depends`) এবং Server-Sent Events (SSE) তৈরিতে।
- **`fastapi-patterns`**: প্রোডাকশন লেভেলের ক্লিন আর্কিটেকচার—সার্ভিস লেয়ার, রিপোজিটরি প্যাটার্ন ও ইন্টিগ্রেশন টেস্টিংয়ে।
- **`fastapi-async-patterns`**: উচ্চ Concurrency নিশ্চিত করতে—Non-blocking ডিবি পুল (asyncpg), asyncio টাস্ক গ্রুপস ও ব্যাকগ্রাউন্ড ওয়ার্কার্স চালাতে।

---

## 6. Systems & Native: Go & Swift

- **`golang-design-patterns`**: Idiomatic Go কোড লিখতে—Functional Options Pattern, Constructor API, Error Wrapping (`errors.Is`/`As`) ও Graceful Shutdown।
- **`golang-popular-libraries`**: গো প্রজেক্টের জন্য পরীক্ষিত প্রোডাকশন-রেডি লাইব্রেরি (Routing, Logging, DB) বেছে নিতে।
- **`golang-documentation`**: গো কোডের সুন্দর Godoc কমেন্ট, এক্সাম্পল টেস্ট এবং প্যাকেজ ডকুমেন্টেশন লিখতে।
- **`write-swift`**: আধুনিক Swift 6 কোড লিখতে—Actor Concurrency, Data-race Safety, Value Types ও ARC মেমোরি ম্যানেজমেন্ট।

---

## 7. AI, Machine Learning & MLOps

- **`ai-ml-development`**: PyTorch বা TensorFlow দিয়ে মডেল ট্রেইনিং, ডেটাসেট পাইপলাইন এবং LLM Fine-tuning-এ।
- **`ml-pipeline`**: MLOps ইনফ্রাস্ট্রাকচার তৈরিতে—Airflow/Kubeflow দিয়ে পাইপলাইন অর্কেস্ট্রেশন, MLflow দিয়ে ট্র্যাকিং ও Feast ফিচার স্টোর সেটআপে।
- **`mle-workflow`**: প্রোডাকশন ML কন্ট্রাক্ট তৈরি, মডেল ভ্যালিডেশন, ড্রিফ্ট মনিটরিং এবং স্বয়ংক্রিয় রোলব্যাক মেকানিজমে।
- **`deploying-machine-learning-models`**: ট্রেইন্ড মডেলকে প্রোডাকশনে সার্ভ করতে (FastAPI, Triton, ONNX Runtime) লো-লেটেন্সি সহকারে।

---

## 8. Testing, QA & DevTools

- **`browser-testing-with-devtools`**: লাইভ Chrome ব্রাউজারে DOM এবং ভিজ্যুয়াল আউটপুট টেস্ট করতে।
- **`chrome-devtools-mcp`**: রিয়েল-টাইম কনসোল এরর ধরা, নেটওয়ার্ক রিকোয়েস্ট ট্র্যাক করা এবং লাইভ CSS ইনস্পেক্ট করতে।
- **`playwright-cli`**: স্বয়ংক্রিয়ভাবে ব্রাউজারে ক্লিক, ফর্ম ফিলআপ এবং End-to-End অটোমেশন টেস্ট চালাতে।
- **`performance-optimization`**: Frontend থেকে Backend পর্যন্ত পুরো সিস্টেমের স্পিড বটলনেক খুঁজে ফিক্স করতে।

---

## 9. Documentation & Copywriting

- **`crafting-effective-readmes`**: যেকোনো নতুন প্রজেক্টের (CLI, লাইব্রেরি বা ওয়েব অ্যাপ) চমৎকার প্রফেশনাল README লিখতে।
- **`readme-optimization`**: বিদ্যমান কোনো README অডিট করে কীভাবে ডেভেলপার কনভার্শন বাড়ানো যায় তা অপটিমাইজ করতে।
- **`no-ai-slop`**: নিজের লেখা ড্রাফট বা আর্টিকেলের নিজস্ব ভয়েস ঠিক রেখে অতিরিক্ত ফুলঝুড়ি ছেঁটে পরিচ্ছন্ন করতে।
- **`humanizer`**: AI-এর মুখস্থ চ্যাটবট স্টাইল ভাষা (Forced triads, Staged openers, ফাঁকা দাবি) দূর করে খাঁটি মানুষের মতো লিখতে।

---

## 10. Mobile-Native & Cloud Operations

- **`mobile-native`**: ফোনে ওয়েবসাইটকে অ্যাপের মতো বানাতে—Touch delay দূর করা, Sticky hover বন্ধ করা, Notch spacing এবং 100vh বাগ ফিক্স করতে।
- **`nextdeploy-cli`**: NextDeploy CLI দিয়ে অ্যাপ ডিপ্লয় ও কনটেইনার কোড সিঙ্ক করতে।
- **`nextdeploy-mcp`**: MCP টুলের মাধ্যমে স্বয়ংক্রিয়ভাবে ক্লাউড ডিপ্লয়মেন্ট চালাতে।
- **`api-recon-and-docs`**: লুকানো এপিআই এন্ডপয়েন্ট বা Swagger ডক খুঁজে অ্যাটাক সারফেস পর্যালোচনা করতে।

---

## Real-World Project Blueprints

### Blueprint 1: E-Commerce CRM Development
1. **Architecture & Seams**: `codebase-design` দিয়ে কাস্টমার ও অর্ডার লজিক আলাদা Deep Module-এ রাখুন।
2. **Backend & Queries**: `django-patterns` + `django-perf-review` (বা `fastapi-patterns`) দিয়ে ডেটাবেস কুয়েরি অপ্টিমাইজড রাখুন।
3. **Admin Dashboard UI**: `frontend-design-complete` দিয়ে ড্যাশবোর্ড থিম এবং `frontend-ui-engineering` দিয়ে কম্পোনেন্ট আর্কিটেকচার সাজান।
4. **Micro-Interactions**: `better-ui` দিয়ে অপটিক্যাল ব্যালেন্স এবং `ask-sonner` দিয়ে ইনস্ট্যান্ট টোস্ট নোটিফিকেশন দিন।
5. **Stress-Testing**: `break-ui` দিয়ে বড় বড় কাস্টমার নাম বা খালি ডেটা দিয়ে টেবিল টেস্ট করুন।
6. **Security & Review**: `security-audit` এবং `code-review-and-quality` চালিয়ে ফাইনাল মার্জ করুন।

### Blueprint 2: High-Converting SaaS Landing Page
1. **Design Foundations**: `frontend-design-complete` + `better-typography` + `better-colors`।
2. **Smooth Motion**: `animate` (হিরো সেকশন এন্ট্রি) + `apple-design` (প্রিমিয়াম গ্লাস কার্ড)।
3. **Mobile Polish**: `mobile-native` (যাতে ফোনে কোনো টাচ ল্যাগ বা হরিজন্টাল স্ক্রল না হয়)।
4. **Copywriting**: `better-writing` + `no-ai-slop` (যাতে লেখা রোবটিক না লেগে কনভার্শন বাড়ায়)।
5. **Performance Audit**: `nextjs-performance` দিয়ে ১০০/১০০ লাইটহাউস স্কোর নিশ্চিত করুন।
