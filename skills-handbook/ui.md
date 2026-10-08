# UI Skills Handbook & Decision Guide

A complete deep-dive guide for all Frontend, UI/UX, Motion, and Design skills installed in the environment.

---

## 1. UI Design Foundations & Visual Direction

নতুন কোনো পেজ, ড্যাশবোর্ড বা কম্পোনেন্টের ডিজাইন শুরু করার সময় এই স্কিলগুলো ব্যবহার করবেন:

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

| Command / Intent | কখন ব্যবহার করবেন |
| :--- | :--- |
| `shape [feature]` | কোড লেখার আগে পুরো UX/UI ফ্লো ও লেআউট প্ল্যান করতে। |
| `document` | বর্তমান কোডবেস থেকে স্বয়ংক্রিয়ভাবে একটি `DESIGN.md` তৈরি করতে। |
| `extract [target]` | বিক্ষিপ্ত কোড থেকে Reusable Tokens ও Components আলাদা করে ডিজাইন সিস্টেমে নিতে। |
| `critique [target]` | হিউরিস্টিক স্কোরিং সহ সম্পূর্ণ UX ডিজাইন রিভিউ পেতে। |
| `polish [target]` | শিপ করার আগের ফাইনাল ফিনিশিং পাস (প্যাডিং, শ্যাডো, অপটিক্যাল ব্যালেন্স)। |
| `bolder [target]` | কোনো ডিজাইন যদি অতিরিক্ত সাদামাটা বা বোরিং মনে হয়, তাকে বোল্ড ও আকর্ষণীয় করতে। |
| `quieter [target]` | কোনো ডিজাইন যদি অতিরিক্ত লাউড বা চটকদার মনে হয়, তাকে মার্জিত ও শান্ত করতে। |
| `distill [target]` | অপ্রয়োজনীয় জটিলতা ও ক্লটার বাদ দিয়ে ডিজাইনের কোর এসেন্স ধরে রাখতে। |
| `harden [target]` | এজ-কেস, এরর স্টেট এবং বিভিন্ন স্ক্রিন সাইজের জন্য প্রোডাকশন-রেডি করতে। |
| `colorize [target]` | কালার প্যালেট নতুন করে সাজাতে বা রিভ্যাম্প করতে। |
| `clarify [target]` | লেআউট হায়ারার্কি এবং ইনফরমেশন আর্কিটেকচার পরিষ্কার করতে। |
| `adapt [target]` | মোবাইল, ট্যাবলেট ও ডেস্কটপের জন্য রেসপন্সিভ অ্যাডাপটেশন করতে। |

---

## 6. Layout Decision Guide: কখন কোনটি বেছে নেবেন?

লেআউট নিয়ে কনফিউশন দূর করতে নিচের রুলগুলো মেনে চলুন:

1. **নতুন পেজের সামগ্রিক রেসপন্সিভ স্ট্রাকচার বানাতে:**
   - ব্যবহার করুন: `better-layout`
   - ফোকাস: Grid columns, Max-width container, Section gaps, Reading order.

2. **React কম্পোনেন্টের ভেতরের লেআউট ও স্টেট ফ্লো বানাতে:**
   - ব্যবহার করুন: `frontend-ui-engineering`
   - ফোকাস: Flexbox alignment, Sub-components composition, Form controls.

3. **মোবাইলে টাচ, নচ ও ফুলস্ক্রিন ফিক্স করতে:**
   - ব্যবহার করুন: `mobile-native`
   - ফোকাস: `100dvh` ফিক্স, iOS Notch padding, Safe-area insets, Disable sticky hover flash.

4. **জটিল ড্যাশবোর্ডের হায়ারার্কি রিফ্যাক্টর করতে:**
   - ব্যবহার করুন: `impeccable` (কমান্ড: `clarify` অথবা `adapt`)
   - ফোকাস: তথ্যের গুরুত্ব অনুযায়ী লেআউট পুনর্বিন্যাস।
