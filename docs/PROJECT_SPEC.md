# از زمین تا روشنایی — Project Specification

**نام فنی پروژه:** `Powerplant-game`  
**نام موقت محصول:** از زمین تا روشنایی  
**نوع محصول:** بازی آموزشی دوبعدی برای Android  
**نوع نیروگاه:** نیروگاه گازی  
**وضعیت:** Concept / Pre-Production  
**نسخه سند:** 0.2

## خلاصه پروژه
یک بازی آموزشی دوبعدی برای فرزندان کارکنان که مسیر ساخت یک نیروگاه گازی را از زمین خالی تا راه‌اندازی، اتصال به شبکه و تحویل پروژه تجربه می‌کنند.

## تصمیمات قطعی فعلی
- گروه سنی: 8 تا 12 سال
- پلتفرم: Android
- سبک: 2D
- نمای اصلی: Top-Down
- موتور بازی: Godot
- توسعه: AI-Assisted / Vibe Coding
- حداکثر مراحل: 10
- زبان MVP: فارسی
- ذخیره: Local Offline Auto-Save
- توزیع: APK روی سرور شرکت + لینک مستقیم/SMS
- شخصیت اصلی: کودک با انتخاب دختر/پسر
- Reward: Stars + Badges + Visible Progress
- پایان بازی: گواهی دیجیتال + Completion Code
- تمرکز: ساخت نیروگاه، نه تعمیرات و بهره‌برداری

## HSE
HSE شامل ایمنی، بهداشت و محیط زیست یک محور سراسری بازی است و نباید محدود به یک مرحله باشد.

موارد نمونه:
- PPE
- فاصله ایمن
- محدوده خطر
- کار ایمن با جرثقیل و ماشین‌آلات
- رفتار ایمن در کارگاه
- توجه به محیط زیست

## Core Gameplay Loop
**Mission → Safety Check → Challenge → Success → Visible Construction Progress → Reward → Next Mission**

## ساختار پیشنهادی مراحل
1. ورود ایمن و آماده‌سازی سایت
2. خاک‌برداری و فونداسیون
3. سازه فلزی
4. ورود و نصب تجهیزات اصلی
5. تجهیزات و سیستم‌های جانبی
6. پایپینگ، کابل و ارتباطات
7. نصب توربین گاز و ژنراتور
8. تست و Pre-Commissioning
9. Commissioning و اتصال به شبکه
10. Final Power-Up / از زمین تا روشنایی

## Voice / Text / Guidance
**Hybrid Voice-over + Minimal Text + Visual Guidance**

Voice-over کوتاه فارسی برای:
- توضیح مأموریت
- نکته مهم HSE
- موفقیت مرحله

## انتخاب شغل والد
ایده پذیرفته شده ولی روش اجرای دقیق هنوز باز است.

اصل فعلی:
- Gameplay برای همه کودکان یکسان بماند.
- انتخاب شغل والد Branch جدا نسازد.
- شخصی‌سازی فقط در پیام، Badge یا توضیح کوتاه باشد.

## Reward نهایی
بعد از Stage 10:
- گواهی «نیروگاه‌ساز کوچک»
- نام کودک
- تاریخ
- امتیاز/Badge
- Completion/Verification Code

نوع هدیه سازمانی یا فیزیکی توسط HR تعیین می‌شود.

## Art Direction
- 2D
- Top-Down
- Friendly Industrial Cartoon
- رنگی و مناسب کودک
- نمایش تدریجی ساخته‌شدن سایت

Art Style دقیق هنوز باز است.

## Open Questions
- نام نهایی محصول
- Art Style دقیق
- روش دقیق شخصی‌سازی بر اساس شغل والد
- روش اعتبارسنجی Completion Code
- نوع Reward سازمانی توسط HR
- جزئیات دقیق Level Design

## مرحله بعدی
**Level Design Specification**

برای هر مرحله باید مشخص شود:
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

## Revision History
| Version | Status | توضیح |
|---|---|---|
| 0.1 | Draft | نسخه اولیه |
| 0.2 | Draft | ثبت تصمیمات جدید پروژه |
