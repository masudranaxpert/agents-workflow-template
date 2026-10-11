# UI Skills Handbook & Decision Guide

A complete deep-dive guide for all Frontend, UI/UX, Motion, and Design skills installed in the environment.

---

## 1. UI Design Foundations & Visual Direction

নতুন কোনো পেজ, ড্যাশবোর্ড বা কম্পোনেন্টের ডিজাইন শুরু করার সময় এই স্কিলগুলো ব্যবহার করবেন:

- **`taste-skill`**: ল্যান্ডিং পেজ, পোর্টফোলিও এবং রিডিজাইনের জন্য অ্যান্টি-স্লপ ফ্রন্টএন্ড ফ্রেমওয়ার্ক। এটি ব্রিফ পড়ে সঠিক ডিজাইন ডিরেকশন ধরে নেয় এবং ৩টি ডায়াল (`DESIGN_VARIANCE`, `MOTION_INTENSITY`, `VISUAL_DENSITY`) দিয়ে জেনেরিক এআই টেমপ্লেট লুক প্রতিরোধ করে।
- **`refactoring-ui`**: অ্যাডাম ওয়াথান ও স্টিভ শোগারের ট্যাকটিক্যাল UI নীতি—আগে সাদা-কালোতে হায়ারার্কি ঠিক করা (Grayscale-first), ফর্ম লেবেল ছোট ও হালকা রাখা, এবং বাটন ও স্পেসিংয়ের সুনির্দিষ্ট স্কেল ব্যবহার করা।
- **`cro-methodology`**: কনভার্সন রেট অপ্টিমাইজেশন—ল্যান্ডিং পেজ, অফার পেজ এবং ই-কমার্স চেকআউট ফানেলে ইউজারদের ড্রপ-অফ বা কার্ট অ্যাবান্ডনমেন্ট কমাতে বৈজ্ঞানিক অডিট।
- **`frontend-design-complete`**: জেনেরিক ChatGPT স্টাইলের সাদামাটা "AI-slop" ডিজাইন (যেমন: সাদা ব্যাকগ্রাউন্ডে পার্পল গ্রেডিয়েন্ট, ক্লিশে কার্ড) বাদ দিয়ে প্রফেশনাল, ইউনিক ও সাহসী আর্ট ডিরেকশন (Brutalist, Luxury, Editorial, Minimalist) তৈরি করতে।
- **`impeccable`**: পুরো UI-এর ভিজ্যুয়াল হায়ারার্কি, ব্যালেন্স এবং ফিনিশিং ক্রাফট টপ-কোম্পানির ডিজাইনারদের মানে নিয়ে যেতে।
- **`better-colors`**: আধুনিক OKLCH কালার প্যালেট তৈরি, ডার্ক মোডের জন্য Semantic Tokens (`--surface`, `--accent`) ডিফাইন এবং WCAG Contrast রেশিও নিশ্চিত করতে।
- **`better-typography`**: Type scale (Heading, Body ফন্ট সাইজ), ফন্ট পেয়ারিং, Line height এবং টেক্সট Truncation সুন্দরভাবে সেট করতে।
- **`better-layout`**: Responsive Grid, Container Spacing, Padding এবং বিভিন্ন Screen Size-এ লেআউট ভেঙে যাওয়া ঠেকাতে।
- **`better-ui`**: নিখুঁত ফিজিক্যাল ডিটেইলস ঠিক করতে—যেমন Concentric Border Radius (`outer = inner + padding`), শক্ত বর্ডারের বদলে Subtle Box Shadow Rings এবং আইকন অপটিক্যাল ব্যালেন্সিং।
- **`better-writing`**: বাটনের টেক্সট, ফিল্ড লেবেল, Empty State মেসেজ এবং এরর নোটিফিকেশন পরিষ্কার ও অ্যাকশনেবল করতে।
- **`better-accessibility`**: Keyboard Focus Navigation (`:focus-visible`), ARIA Labels এবং টাচ স্ক্রিনে মিনিমাম 44x44px Tap Target নিশ্চিত করতে।
- **`better-interface`**: কালার, টাইপোগ্রাফি, স্পেসিং, মাইক্রোকপি এবং অ্যাক্সেসিবিলিটি—এই সব কটি বিষয় একবারে কমপ্রিহেনসিভ রিভিউ করতে।
- **`build-design`**: Figma স্ক্রিনশট বা ডিজাইনের ছবি দেখে সরাসরি আপনার কোডবেসের বিদ্যমান টোকেন দিয়ে Pixel-perfect কোড লিখতে।

---

## 2. Component Engineering & Frameworks

ডিজাইন ডিরেকশন ঠিক হওয়ার পর যখন সরাসরি কোড লিখবেন:

- **`frontend-ui-engineering`**: ক্লিন React কোড আর্কিটেকচার। Configuration-এর বদলে Composition (`<Card><CardHeader/></Card>`) প্রাধান্য দেওয়া, কাস্টম হুক ও ফর্ম স্টেট হ্যান্ডলিং।
- **`frontend-patterns`**: React ও Next.js কম্পোনেন্টে অপ্রয়োজনীয় Re-render বন্ধ করতে এবং স্টেট ফ্লো পরিচ্ছন্ন রাখতে।
- **`tailwind-4-docs`**: Tailwind CSS v4-এর আধুনিক `@theme` কনফিগারেশন, Container Queries এবং নতুন CSS-first ইউটিলিটি ব্যবহার করতে।
- **`pick-ui-library`**: আপনার প্রজেক্টের জন্য কোন Headless বা স্টাইলড কম্পোনেন্ট লাইব্রেরি সেরা (shadcn/ui, Radix, Base UI ইত্যাদি) তা নিরপেক্ষভাবে বেছে নিতে।
- **`react`**: JSON স্পেসিফিকেশন থেকে ডায়নামিক React কম্পোনেন্ট রেন্ডার করতে (`@json-render/react`)।
- **`react-components`**: Stitch ক্যানভাসের সাথে মডুলার React কম্পোনেন্ট সিঙ্ক করতে।
- **`react-doctor`**: React কোডবেসে Hook Rules ভায়োলেশন, স্টেট মিউটেশন বা পারফরম্যান্স লিক স্ক্যান ও ফিক্স করতে।
- **`htmx`**: ভারী রিঅ্যাক্ট/এসপিএ ফ্রেমওয়ার্ক ছাড়া সরাসরি সার্ভার-সাইড HTML সোয়াপ দিয়ে ডায়নামিক ইন্টারঅ্যাকশন তৈরি করতে।
- **`alpine-js`**: লাইটওয়েট ব্যাকএন্ড টেমপ্লেটে (Django বা Blade) ড্রপডাউন, মোডাল বা টগলের মতো হালকা রিয়্যাক্টিভ কাজ করতে।

---

## 3. Motion, Animation & Polish

UI-তে প্রিমিয়াম অনুভূতি এবং মসৃণ ইন্টারঅ্যাকশন দিতে:

- **`animate`**: স্ক্র্যাচ থেকে যেকোনো ওয়েব অ্যানিমেশন তৈরি—Spring Physics, Cubic-bezier Easing, Entry/Exit অ্যানিমেশন এবং Interruptible Transitions বানাতে।
- **`emil-design-eng`**: Emil Kowalski-র ডিজাইন ফিলোসফি—বাটনের ক্লিক ফিডব্যাক, কার্ডের সূক্ষ্ম হভার এফেক্ট এবং সফটওয়্যারের মাইক্রো-ডিটেইলস নিখুঁত করতে।
- **`apple-design`**: অ্যাপল স্টাইলের ফ্লুইড জেসচার, Translucent Glass Materials (`backdrop-filter`) এবং মোমেন্টাম স্প্রিং বটম-শিট বানাতে।
- **`animate-expo`**: React Native / Expo মোবাইল অ্যাপে Reanimated ও Haptic Feedback দিয়ে মোশন তৈরি করতে।
- **`animation-vocabulary`**: কোনো অ্যানিমেশন মাথায় আছে কিন্তু টেকনিক্যাল নাম জানেন না (যেমন: "Rubber-banding", "Pop in")—সঠিক নাম রিভার্স-লুকআপ করতে।
- **`find-animation-opportunities`**: পুরো কোডবেস স্ক্যান করে কোথায় কোথায় সূক্ষ্ম মোশন দিলে সাইটটি আরও ইন্টারঅ্যাক্টিভ লাগবে তা খুঁজে বের করতে।
- **`review-animations`**: কোডের অ্যানিমেশন পারফরম্যান্স চেক করতে—GPU Compositor thread ব্যবহার হচ্ছে কিনা এবং ফ্রেম ড্রপ হচ্ছে কিনা তা অডিট করতে।
- **`improve-animations`**: বিদ্যমান অ্যাপের মোশন আর্কিটেকচার রিফ্যাক্টর করার জন্য ধাপে ধাপে রোডম্যাপ তৈরি করতে।
- **`ask-sonner`**: চমৎকার ও রেসপন্সিভ Sonner Toast নোটিফিকেশন যুক্ত করতে।
- **`vercel-react-view-transitions`**: এক পেজ থেকে অন্য পেজে যাওয়ার সময় মসৃণ View Transitions এবং Shared Element ট্রানজিশন দিতে।

---

## 4. UI Testing, Variations & Stress-Testing

শিপ করার আগে কম্পোনেন্ট রিয়েল ডেটাতে টিকে থাকে কিনা যাচাই করতে:

- **`break-ui` (Emil Kowalski)**: কম্পোনেন্টের ভেতরেই একটি টগল বসিয়ে বাস্তবজীবনের চরম বাজে ডেটা (অতিরিক্ত বড় নাম, ১টি আইটেম, শূন্য ডেটা, আনব্রেকেবল ইমেইল) দিয়ে দেখতে লেআউট নষ্ট হয় কিনা।
- **`break` (Jakub Krehel)**: একটি আলাদা টেস্ট পেজ বানিয়ে কম্পোনেন্টের সব ভিজ্যুয়াল স্টেট (hover, active, disabled, focus) পাশাপাশি বড় ক্যানভাসে দেখতে।
- **`variant`**: একই কম্পোনেন্টের ৩–৪টি ভিন্ন ডিজাইন ভ্যারিয়েশন তৈরি করে ক্লায়েন্ট বা নিজের চোখের সামনে তুলনা করতে।
- **`design-lab`**: প্রজেক্ট স্ট্যাক ও টোকেন বুঝে একবারে ৫টি সম্পূর্ণ ভিন্ন ডিজাইন ভ্যারিয়েন্ট তৈরি করে এবং ব্রাউজারে লাইভ ফিডব্যাক ওভারলে সুইচার দিয়ে সহজে তুলনা ও পছন্দ করতে দেয়।
- **`prototype`**: কোনো নতুন আইডিয়া দ্রুত কোড করে ২-৩টি সম্পূর্ণ ভিন্ন কার্যপদ্ধতি পরখ করে দেখতে।
- **`state-machine`**: জটিল কম্পোনেন্টের সব কটি পসিবল স্টেট (Loading, Error, Empty, Success, Editing) একটি সুইচার দিয়ে ড্রাইভ করতে।
- **`explain-interface`**: ইন্টারনেটের কোনো সুন্দর সাইটের অ্যানিমেশন বা ইন্টারফেস কীভাবে তৈরি হয়েছে তা স্ক্রিনশট বা লিংক দিয়ে রিভার্স-ইঞ্জিনিয়ারিং করতে।

---

## 5. Impeccable Deep Dive: Modes & Commands

`impeccable` হলো একটি হাই-এন্ড ডিজাইন ডিরেক্টর স্কিল। সাধারণ স্কিলের মতো এটি শুধু কোড লিখে না, বরং প্রজেক্টের কনটেক্সট বুঝে সুনির্দিষ্ট মোড ও কমান্ডে কাজ করে।

### Surface Modes (কাজের ধরন অনুযায়ী মোড নির্বাচন)
- **Persuade Mode**: Landing Page, Marketing, Pricing পেজের জন্য। উদ্দেশ্য: ইউজারের মনোযোগ আকর্ষণ ও অ্যাকশনে কনভার্ট করা।
- **Operate Mode**: Admin Dashboard, Data Table, Tools, Settings পেজের জন্য। উদ্দেশ্য: দ্রুত কাজ শেষ করা (Scannability, Efficiency)।
- **Read Mode**: Documentation, Blog, Help Center-এর জন্য। উদ্দেশ্য: পড়ার আরাম ও পরিষ্কার কাঠামো।
- **Experience Mode**: Portfolio, Showcase, Gallery-এর জন্য। উদ্দেশ্য: প্রথম ভিউপোর্টেই ভিজ্যুয়াল আর্ট প্রাধান্য পাবে।

### Useful Sub-Commands & Prompts
আপনি প্রম্পটে সরাসরি নিচের কাজগুলো মেনশন করে `impeccable` চালাতে পারেন:

| Command | Category | বিবরণ (বাংলা) | Description (English) | Reference |
| :--- | :--- | :--- | :--- | :--- |
| `craft [feature]` | Build | নতুন কাজের রিকোয়েস্টের পুরনো ফরম্যাট (Deprecated) | Deprecated alias for an ordinary new-work request | [reference/craft.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/craft.md) |
| `shape [feature]` | Build | কোড লেখার আগে পুরো UX/UI কাঠামো ও ফ্লো প্ল্যান করা | Plan UX/UI before writing code | [reference/shape.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/shape.md) |
| `init` | Build | প্রজেক্টের স্থায়ী কনটেক্সট `PRODUCT.md`-এ সংরক্ষণ করা | Capture durable product context in PRODUCT.md | [reference/init.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/init.md) |
| `document` | Build | বিদ্যমান কোডবেস বিশ্লেষণ করে স্বয়ংক্রিয়ভাবে `DESIGN.md` তৈরি করা | Generate DESIGN.md from existing project code | [reference/document.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/document.md) |
| `extract [target]` | Build | কোড থেকে Reusable Tokens ও Components আলাদা করে ডিজাইন সিস্টেমে নেওয়া | Pull reusable tokens and components into design system | [reference/extract.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/extract.md) |
| `critique [target]` | Evaluate | হিউরিস্টিক স্কোরিংসহ নিরপেক্ষ ও গভীর UX ডিজাইন রিভিউ পাওয়া | UX design review with heuristic scoring | [reference/critique.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/critique.md) |
| `audit [target]` | Evaluate | টেকনিক্যাল কোয়ালিটি চেক (এক্সেসিবিলিটি, পারফরম্যান্স, রেসপন্সিভনেস) | Technical quality checks (a11y, perf, responsive) | [reference/audit.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/audit.md) · native: [reference/audit.native.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/audit.native.md) |
| `polish [target]` | Refine | শিপ বা রিলিজ করার আগের ফাইনাল কোয়ালিটি ফিনিশিং পাস | Final quality pass before shipping | [reference/polish.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/polish.md) |
| `bolder [target]` | Refine | অতিরিক্ত সাদামাটা বা বোরিং ডিজাইনকে বোল্ড ও আকর্ষণীয় করা | Amplify safe or bland designs | [reference/bolder.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/bolder.md) |
| `quieter [target]` | Refine | অতিরিক্ত লাউড বা চোখে লাগা ডিজাইনকে শান্ত ও মার্জিত করা | Tone down aggressive or overstimulating designs | [reference/quieter.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/quieter.md) |
| `distill [target]` | Refine | অপ্রয়োজনীয় জটিলতা ছেঁটে ফেলে ডিজাইনের মূল এসেন্স ধরে রাখা | Strip to essence, remove complexity | [reference/distill.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/distill.md) |
| `harden [target]` | Refine | প্রোডাকশন-রেডি করা: এরর স্টেট, আন্তর্জাতিকীকরণ (i18n), এজ-কেস হ্যান্ডলিং | Production-ready: errors, i18n, edge cases | [reference/harden.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/harden.md) |
| `onboard [target]` | Refine | ফার্স্ট-রান ফ্লো, Empty States এবং ইউজার অ্যাক্টিভেশন ডিজাইন করা | Design first-run flows, empty states, activation | [reference/onboard.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/onboard.md) |
| `animate [target]` | Enhance | উদ্দেশ্যমূলক অ্যানিমেশন ও মসৃণ ট্রানজিশন যোগ করা | Add purposeful animations and motion | [reference/animate.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/animate.md) |
| `colorize [target]` | Enhance | একঘেয়ে মোনোক্রোম্যাটিক UI-তে কৌশলগত অ্যাকসেন্ট কালার ছড়ানো | Add strategic color to monochromatic UIs | [reference/colorize.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/colorize.md) |
| `typeset [target]` | Enhance | ফন্ট নির্বাচন, হায়ারার্কি, সাইজিং ও টাইপোগ্রাফি রিদম উন্নত করা | Improve typography hierarchy and fonts | [reference/typeset.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/typeset.md) |
| `layout [target]` | Enhance | স্পেসিং, প্যাডিং, কন্টেইনার রিদম ও ভিজ্যুয়াল হায়ারার্কি ফিক্স করা | Fix spacing, rhythm, and visual hierarchy | [reference/layout.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/layout.md) |
| `delight [target]` | Enhance | ইন্টারফেসে ব্যক্তিত্ব ও স্মরণীয় মাইক্রো-টাচ যোগ করা | Add personality and memorable touches | [reference/delight.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/delight.md) |
| `overdrive [target]` | Enhance | প্রচলিত ডিজাইনের গণ্ডি ভেঙে চরম এক্সপেরিমেন্টাল রূপ দেওয়া | Push past conventional limits | [reference/overdrive.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/overdrive.md) |
| `clarify [target]` | Fix | বিভ্রান্তিকর UX কপি, লেবেল, বাটন টেক্সট ও এরর মেসেজ সহজবোধ্য করা | Improve UX copy, labels, and error messages | [reference/clarify.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/clarify.md) |
| `adapt [target]` | Fix | মোবাইল, ট্যাবলেট, ডেস্কটপের মতো ভিন্ন স্ক্রিন সাইজের জন্য নিখুঁত অ্যাডাপ্ট করা | Adapt for different devices and screen sizes | [reference/adapt.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/adapt.md) · native: [reference/adapt.native.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/adapt.native.md) |
| `optimize [target]` | Fix | UI রেন্ডারিং ল্যাগ ও ফ্রন্টএন্ড পারফরম্যান্স সমস্যা ডায়াগনোজ ও ফিক্স করা | Diagnose and fix UI performance | [reference/optimize.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/optimize.md) |
| `live` | Iterate | ব্রাউজারে রিয়েল-টাইমে উপাদান সিলেক্ট করে বিকল্প ডিজাইন নিয়ে এক্সপেরিমেন্ট করা | Visual variant mode: pick elements in the browser, iterate on alternatives | [reference/live.md](https://github.com/pbakaus/impeccable/blob/main/skill/reference/live.md) |
| `generate [n] [action] [element]` | Iterate | ব্রাউজারে দেখতে স্বয়ংক্রিয়ভাবে একাধিক বিকল্প ভ্যারিয়েন্ট জেনারেট করা | Variants, versions, or alternatives of a named element to choose from in the live browser; no manual picking |

---

## 6. Layout Decision Guide: কখন কোনটি বেছে নেবেন?

লেআউট নিয়ে কনফিউশন দূর করতে নিচের রুলগুলো মেনে চলুন:

1. **ল্যান্ডিং পেজ, পোর্টফোলিও বা রিডিজাইন বানাতে:**
   - ব্যবহার করুন: `taste-skill`
   - কেন: `impeccable` মাঝেমধ্যে ল্যান্ডিং পেজে অতিরিক্ত জেনেরিক বা খাপছাড়া ডিজাইন করে ফেলে। `taste-skill` এর ৩টি ডায়াল (Variance, Motion, Density) এবং ব্রিফ ইনফারেন্স দিয়ে সুনির্দিষ্ট আর্ট ডিরেকশন ধরে রাখে।

2. **ড্যাশবোর্ড, সেটিংস, টুলস বা প্রোডাক্ট UI বানাতে:**
   - ব্যবহার করুন: `impeccable` (Operate মোড)
   - ফোকাস: ফাংশনাল ও শান্ত ইন্টারফেস, জটিল ফর্ম ও টেবিল লেআউট।

3. **নতুন পেজের সামগ্রিক রেসপন্সিভ স্ট্রাকচার বানাতে:**
   - ব্যবহার করুন: `better-layout`
   - ফোকাস: Grid columns, Max-width container, Section gaps, Reading order.

4. **React কম্পোনেন্টের ভেতরের লেআউট ও স্টেট ফ্লো বানাতে:**
   - ব্যবহার করুন: `frontend-ui-engineering`
   - ফোকাস: Flexbox alignment, Sub-components composition, Form controls.

5. **মোবাইলে টাচ, নচ ও ফুলস্ক্রিন ফিক্স করতে:**
   - ব্যবহার করুন: `mobile-native`
   - ফোকাস: `100dvh` ফিক্স, iOS Notch padding, Safe-area insets, Disable sticky hover flash.

6. **জটিল ড্যাশবোর্ডের হায়ারার্কি রিফ্যাক্টর করতে:**
   - ব্যবহার করুন: `impeccable` (কমান্ড: `clarify` অথবা `adapt`)
   - ফোকাস: তথ্যের গুরুত্ব অনুযায়ী লেআউট পুনর্বিন্যাস।

7. **ফর্ম, টেবিল ও ডেটা উইজেটের ভিজ্যুয়াল হায়ারার্কি নিখুঁত করতে:**
   - ব্যবহার করুন: `refactoring-ui`
   - ফোকাস: লেবেল ডিম্পাসাইজ করা, বাটন হায়ারার্কি (Primary/Secondary), ৩-লেভেল সাইজিং ও ফিক্সড স্পেসিং স্কেল।

8. **ই-কমার্স চেকআউট ও কনভার্সন ফানেল অপ্টিমাইজ করতে:**
   - ব্যবহার করুন: `cro-methodology`
   - ফোকাস: ঘর্ষণ ও দ্বিধা দূর করা, ভ্যালু প্রোপোজিশন স্পষ্ট করা, ড্রপ-অফ পয়েন্ট ফিক্স করা।
