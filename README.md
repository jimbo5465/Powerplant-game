Powerplant-game

از زمین تا روشنایی

یک بازی آموزشی دوبعدی برای کودکان 8 تا 12 سال که مسیر ساخت یک نیروگاه را از زمین خالی تا راه‌اندازی، اتصال به شبکه و تحویل پروژه تجربه می‌کنند.

وضعیت پروژه

Concept / Pre-Production

پروژه در مرحله طراحی مفهومی و تدوین Specification قرار دارد.

هدف پروژه

هدف بازی ترکیب سه عنصر اصلی است:

- سرگرمی
- آموزش
- آشنایی کودک با پروژه نیروگاهی و نقش شغلی پدر یا مادر

بازیکن در طول بازی یک پروژه نیروگاهی را از مرحله تحویل زمین و عملیات عمرانی تا نصب تجهیزات، راه‌اندازی و اتصال به شبکه پیش می‌برد.

هدف، ساخت یک شبیه‌ساز تخصصی نیروگاه نیست؛ بلکه ایجاد یک تجربه ساده، جذاب و قابل‌فهم برای کودک است.

کانسپت اصلی

بازیکن بازی را با یک سایت تقریباً خالی شروع می‌کند.

با انجام هر مرحله، بخشی از نیروگاه ساخته می‌شود:

زمین خالی → آماده‌سازی سایت → فونداسیون → سازه → تجهیزات → ارتباطات → توربین و ژنراتور → تست → راه‌اندازی → اتصال به شبکه

مهم‌ترین پاداش بازیکن، دیدن ساخته‌شدن تدریجی نیروگاه است.

ویژگی‌های فعلی

- پلتفرم هدف: Android
- بازی کاملاً 2D
- حداکثر 10 مرحله
- گروه سنی اولیه: 8 تا 12 سال
- مراحل کوتاه و Mission-Based
- Mini Games ساده
- طراحی مناسب برای Vibe Coding
- توسعه با کمک ابزارهای AI
- تمرکز روی ساخت نیروگاه، نه تعمیرات و بهره‌برداری
- سیستم Stars و Badges
- نمایش Progress نیروگاه
- ارتباط مراحل با تخصص‌های مختلف کارکنان
- گواهی دیجیتال پایان بازی

ژانر

2D Construction Adventure + Mini Games + Light Simulation

تعریف ساده‌تر:

«کودک با انجام مجموعه‌ای از مأموریت‌ها و مینی‌گیم‌های کوتاه، یک نیروگاه را مرحله‌به‌مرحله می‌سازد.»

Core Gameplay Loop

Mission
   ↓
Challenge
   ↓
Success
   ↓
Visible Construction Progress
   ↓
Reward
   ↓
Next Mission

Working Title

از زمین تا روشنایی

نام فعلی موقت است و می‌تواند در مراحل بعد تغییر کند.

مستندات پروژه

- "Project Specification" (docs/PROJECT_SPEC.md)
- "Game Design" (docs/GAME_DESIGN.md)
- "Level Design" (docs/LEVEL_DESIGN.md)
- "Art Direction" (docs/ART_DIRECTION.md)
- "Technical Specification" (docs/TECHNICAL_SPEC.md)

سند اصلی و مرجع فعلی پروژه:

"docs/PROJECT_SPEC.md"

ساختار پیشنهادی Repository

Powerplant-game/
│
├── README.md
│
├── docs/
│   ├── PROJECT_SPEC.md
│   ├── GAME_DESIGN.md
│   ├── LEVEL_DESIGN.md
│   ├── ART_DIRECTION.md
│   └── TECHNICAL_SPEC.md
│
├── game/
│
├── assets/
│   ├── characters/
│   ├── environments/
│   ├── equipment/
│   ├── ui/
│   └── audio/
│
├── prototypes/
│
└── research/

اصول طراحی

1. Fun First, Learning Embedded
   بازی باید اول سرگرم‌کننده باشد و آموزش در دل Gameplay قرار بگیرد.

2. One Level, One Main Mechanic
   هر مرحله فقط یک مکانیک اصلی و قابل‌فهم داشته باشد.

3. Visible Progress
   بازیکن باید نتیجه هر مرحله را مستقیماً در نیروگاه ببیند.

4. Short Sessions
   مراحل کوتاه و قابل اتمام باشند.

5. Increasing Excitement
   هیجان بازی در مراحل پایانی بیشتر شود.

6. Low Technical Complexity
   طراحی باید متناسب با توسعه سریع و AI-Assisted باشد.

7. Humanize Engineering
   بازی فقط درباره ماشین‌آلات نیست؛ درباره آدم‌هایی است که نیروگاه را می‌سازند.

محدوده فعلی پروژه

موارد زیر فعلاً خارج از Scope هستند:

- 3D
- Multiplayer
- Open World
- City Builder کامل
- Simulation صنعتی دقیق
- Loot Box
- تبلیغات
- In-App Purchase
- Daily Reward
- تعمیرات و نگهداری زمان بهره‌برداری
- NPC AI پیچیده
- Backend سنگین

مرحله بعدی

قدم بعدی پروژه:

Level Design Specification

برای هر مرحله باید موارد زیر مشخص شوند:

- Story Context
- Learning Objective
- Mission
- Gameplay Mechanic
- Interaction
- Win Condition
- Retry Condition
- Reward
- Visual Changes
- Parent Job Connection
- Required Assets
- Development Complexity
