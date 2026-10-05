# Powerplant-game

## از زمین تا روشنایی

یک بازی آموزشی دوبعدی برای کودکان ۸ تا ۱۲ سال که مسیر ساخت یک **نیروگاه گازی** را از زمین خالی تا راه‌اندازی، اتصال به شبکه و تحویل پروژه تجربه می‌کنند.

## وضعیت پروژه

**Concept / Pre-Production**

پروژه در مرحله طراحی مفهومی و تدوین Specification قرار دارد. تمرکز فعلی روی **Level Design Specification** است.

## هدف پروژه

هدف بازی ترکیب این عناصر است:

- سرگرمی
- آموزش فرایند ساخت نیروگاه
- آشنایی کودک با شغل و محیط کاری پدر یا مادر
- انتقال فرهنگ HSE شامل ایمنی، بهداشت و محیط زیست
- ایجاد یک تجربه سازمانی مثبت برای خانواده کارکنان

هدف، ساخت یک شبیه‌ساز تخصصی نیروگاه نیست؛ بلکه ایجاد یک تجربه ساده، جذاب، کودک‌فهم و قابل توسعه با کمک AI است.

## کانسپت اصلی

بازیکن بازی را با یک سایت تقریباً خالی شروع می‌کند.

با انجام هر مرحله، بخشی از نیروگاه ساخته می‌شود:

**زمین خالی → آماده‌سازی سایت → فونداسیون → سازه → تجهیزات → سیستم‌ها و ارتباطات → توربین گاز و ژنراتور → تست → راه‌اندازی → اتصال به شبکه**

مهم‌ترین پاداش بازیکن، دیدن ساخته‌شدن تدریجی نیروگاه است.

## ویژگی‌های فعلی

- پلتفرم هدف: Android
- بازی کاملاً 2D
- نمای اصلی: Top-Down
- نوع نیروگاه: Gas Power Plant
- حداکثر ۱۰ مرحله
- گروه سنی: ۸ تا ۱۲ سال
- مراحل کوتاه و Mission-Based
- Mini Games ساده
- موتور بازی: Godot
- توسعه با رویکرد AI-Assisted / Vibe Coding
- تمرکز روی ساخت نیروگاه، نه تعمیرات و بهره‌برداری
- HSE به‌عنوان محور سراسری تمام مراحل
- سیستم Stars و Badges
- نمایش Visible Progress نیروگاه
- Local Offline Auto-Save
- Voice-over کوتاه فارسی + متن کم + Visual Guidance
- ارتباط مراحل با تخصص‌های مختلف کارکنان
- شخصیت اصلی کودک با انتخاب دختر یا پسر
- گواهی دیجیتال پایان بازی
- Completion / Verification Code
- توزیع اولیه با APK از طریق سرور شرکت و لینک مستقیم/SMS

## ژانر

**2D Construction Adventure + Mini Games + Light Simulation**

تعریف ساده‌تر:

> کودک با انجام مجموعه‌ای از مأموریت‌ها و مینی‌گیم‌های کوتاه، یک نیروگاه گازی را مرحله‌به‌مرحله می‌سازد.

## Core Gameplay Loop

```text
Mission
   ↓
Safety Check
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
```

## HSE

HSE فقط یک مرحله جداگانه نیست؛ باید در تمام بازی حضور داشته باشد.

نمونه‌ها:

- انتخاب PPE مناسب
- رعایت فاصله ایمن
- تشخیص رفتار ناایمن
- توجه به محدوده خطر
- ایمنی هنگام کار با جرثقیل و ماشین‌آلات
- توجه ساده به محیط زیست و نظم کارگاهی

## شخصیت اصلی

شخصیت اصلی یک کودک است.

در ابتدای بازی:

- بازیکن می‌تواند شخصیت دختر یا پسر را انتخاب کند.
- «مهندس کوچک» فعلاً یک عنوان مفهومی و Placeholder است.
- نام نهایی محصول و شخصیت بعداً تعیین می‌شود.

## راهنمایی و آموزش

روش فعلی:

**Hybrid Voice-over + Minimal Text + Visual Guidance**

Voice-over کوتاه فارسی برای:

- توضیح مأموریت
- نکته مهم HSE
- موفقیت و عبور به مرحله بعد

همراه با:

- متن کوتاه
- فلش
- Highlight
- راهنمای تصویری

## ارتباط با شغل والد

ایده انتخاب حوزه کاری والد پذیرفته شده، اما روش اجرای دقیق هنوز باز است.

اصل فعلی:

- Gameplay برای همه کودکان یکسان بماند.
- انتخاب شغل والد Branch جداگانه نسازد.
- شخصی‌سازی فقط در پیام، Badge یا توضیح کوتاه انجام شود.

## Progress و ذخیره‌سازی

نسخه اول از **Local Offline Progress System** استفاده می‌کند.

- Auto Save بعد از پایان هر مرحله
- ذخیره آخرین مرحله بازشده
- ذخیره Stars و Badges
- امکان Replay مراحل قبلی
- Locked بودن مراحل آینده
- بدون Login
- بدون Backend
- بدون Cloud Save در MVP

## Reward نهایی

در پایان بازی کودک یک گواهی دیجیتال دریافت می‌کند.

عنوان فعلی پیشنهادی:

**نیروگاه‌ساز کوچک**

گواهی می‌تواند شامل موارد زیر باشد:

- نام کودک
- تاریخ
- امتیاز
- Badgeها
- Completion / Verification Code

نوع هدیه فیزیکی یا سازمانی توسط HR تعیین می‌شود.

## توزیع نسخه Android

روش فعلی برای MVP:

1. تولید APK
2. قرار دادن فایل روی سرور یا زیرساخت شرکت
3. ارسال لینک دانلود برای خانواده‌ها، مثلاً از طریق SMS
4. نصب مستقیم روی گوشی Android

انتشار عمومی در Google Play یا Myket فعلاً جزو Scope نسخه اول نیست.

## Working Title

**از زمین تا روشنایی**

نام فعلی موقت است و می‌تواند در مراحل بعد تغییر کند.

## مستندات پروژه

- [Project Specification](docs/PROJECT_SPEC.md)
- [Game Design](docs/GAME_DESIGN.md)
- [Level Design](docs/LEVEL_DESIGN.md)
- [Art Direction](docs/ART_DIRECTION.md)
- [Technical Specification](docs/TECHNICAL_SPEC.md)

سند اصلی مرجع پروژه:

`docs/PROJECT_SPEC.md`

## اصول طراحی

1. **Fun First, Learning Embedded**  
   بازی باید اول سرگرم‌کننده باشد و آموزش در دل Gameplay قرار بگیرد.

2. **Safety Embedded Everywhere**  
   ایمنی، بهداشت و محیط زیست باید در تمام مراحل حضور داشته باشند.

3. **One Level, One Main Mechanic**  
   هر مرحله فقط یک مکانیک اصلی و قابل‌فهم داشته باشد.

4. **Visible Progress**  
   بازیکن باید نتیجه هر مرحله را مستقیماً در سایت نیروگاه ببیند.

5. **Short Sessions**  
   مراحل کوتاه و قابل اتمام باشند.

6. **Increasing Excitement**  
   هیجان بازی در مراحل پایانی بیشتر شود.

7. **Low Technical Complexity**  
   طراحی باید متناسب با توسعه سریع و AI-Assisted باشد.

8. **Humanize Engineering**  
   بازی فقط درباره ماشین‌آلات نیست؛ درباره آدم‌هایی است که نیروگاه را می‌سازند.

9. **Offline First**  
   نسخه اول بدون وابستگی به Backend یا Login کار کند.

## محدوده فعلی پروژه

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
- Cloud Save
- انتشار عمومی App Store در MVP

## مرحله بعدی

قدم بعدی پروژه:

**Level Design Specification**

برای هر مرحله باید موارد زیر مشخص شوند:

- Story Context
- Construction Phase
- Learning Objective
- HSE Objective
- Mission
- Gameplay Mechanic
- Interaction
- Voice-over / Guidance
- Win Condition
- Retry Condition
- Reward
- Visual Changes
- Parent Job Connection
- Required Assets
- Development Complexity
