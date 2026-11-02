# 🧠 Idea Drill-Through (AI Checklist Architect v2.1)

[![Platform: ChatGPT](https://img.shields.io/badge/ChatGPT-Custom_GPT_%26_Projects-10a37f?style=flat-square)](#۱-نصب-در-chatgpt-custom-gpt--projects)
[![Platform: Claude](https://img.shields.io/badge/Claude-Projects_%26_Claude_Code-d97757?style=flat-square)](#۲-نصب-در-claude-claude-projects--claude-code)
[![Platform: Gemini](https://img.shields.io/badge/Gemini-Gems_%26_AI_Studio-4285f4?style=flat-square)](#۳-نصب-در-google-gemini-gems--ai-studio)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

**ماشین وضعیت ۵ مرحلهای (5-Gate State Machine)** برای تبدیل ایدههای خام، فرضیههای تحلیلی و نیازمندیهای کسبوکار به **پرامپتهای مهندسیشده دقیق (Master Prompts)** و **گزارشهای استراتژیک ممیزیشده**.

---

## 💡 چرا این اسکیل ساخته شده است؟

کار کردن معمولی با مدلهای زبانی (ChatGPT, Claude, Gemini) سه باگ شناختی بزرگ دارد:
1. **تنبلی شناختی (Cognitive Offloading):** کاربر بدون اینکه خودش فرضیه اولیهای داشته باشد، فکر کردن را کامل به هوش مصنوعی واگذار میکند و خروجیهای کلیشهای میگیرد.
2. **چاپلوسی مدل (RLHF Sycophancy):** مدلهای زبانی به دلیل آموزش RLHF تمایل دارند ایدههای کاربر را تایید و تحسین کنند، نه اینکه باگهای منطقی و مالی آن را به چالش بکشند.
3. **توهم داده (Data Hallucination):** مدلها در مواجهه با دادههای ناقص، بهجای اعلام عدم قطعیت، اعداد و فرضیات پنهان میسازند.

**Idea Drill-Through** با یک موتور امتیازدهی کمی ($CI_g$ از ۰ تا ۱۰۰) شما را قدمبهقدم از **۵ دروازه کنترلی** عبور میدهد و تا زمانی که شفافیت نیازمندی شما در هر دروازه به امتیاز `85/100` نرسد، اجازه عبور به مرحله بعد را نمیدهد.

---

## 🔄 معماری ۵ دروازه (The 5 Sequential Gates)

| دروازه | عنوان | هدف اصلی | شرط توقف (Hard Stop / Rules) |
| :--- | :--- | :--- | :--- |
| **Gate 1** | **ممیزی شناختی و قفل فرضیه** | ثبت فرضیه مستقل انسانی، KPI اصلی، تقسیم کار Centaur و بررسی حریم خصوصی | اگر کاربر فرضیه اولیه نداشته باشد ($C_{1.1}=0$)، سیستم متوقف میشود. |
| **Gate 2** | **معماری ساختاری و Map-Reduce** | تعیین نقش واقعگرایانه، کاتالوگ/نرخنامه، تحلیل دو مرحلهای (Map-Reduce) و ساختار داده | الزام به تحلیل مجزای هر منبع قبل از ترکیب نتایج. |
| **Gate 3** | **مقیدسازی سختگیرانه (Grounding)** | قفل کردن منبع حقیقت، قوانین ایزولاسیون دامنه، تگ `[اطلاعات ناموجود]` و اسکیمای خروجی | ممنوعیت مطلق حدس زدن اعداد ناموجود. |
| **Gate 4** | **کالیبراسیون ضدچاپلوسی و کامپایل** | حذف ضمایر مالکیت، تشکیل شورای ۴ نفره منتقدان (Adversarial Council) و **تولید پرامپت نهایی** | حذف تعارفات و حفظ تضاد منافع واقعی بین اعضای شورا. |
| **Gate 5** | **ممیزی ۲ دقیقهای پس از اجرا** | افشای فرضیات پنهان مدل، راستیآزمایی دستی اعداد، و ثبت تصمیم نهایی توسط انسان | تصمیمگیری نهایی بر عهده انسان است، نه هوش مصنوعی. |

---

## 🚀 راهنمای نصب و استفاده در پلتفرمهای مختلف

### ۱. نصب در ChatGPT (Custom GPT & Projects)
**روش اول (ساخت Custom GPT قابل اشتراکگذاری با لینک):**
1. وارد بخش **Explore GPTs -> Create** در ChatGPT شوید.
2. تب **Configure** را انتخاب کنید.
3. نام را `Idea Drill-Through Architect` بگذارید.
4. محتوای فایل [`core/UNIVERSAL_SYSTEM_PROMPT.md`](core/UNIVERSAL_SYSTEM_PROMPT.md) را کپی کرده و در باکس **Instructions** قرار دهید.
5. در بخش Capabilities، تیک **Code Interpreter & Data Analysis** را فعال کنید (برای تحلیل دقیق فایلهای اکسل و CSV در دروازه ۲).
6. روی **Create** کلیک کرده و لینک آن را با تیم خود به اشتراک بگذارید.

**روش دوم (استفاده در ChatGPT Projects):**
* یک Project جدید بسازید و محتوای فایل `core/UNIVERSAL_SYSTEM_PROMPT.md` را در بخش **Project Instructions** قرار دهید.

---

### ۲. نصب در Claude (Claude Projects & Claude Code)
**روش اول (Claude.ai Projects - پیشنهادی):**
1. در وبسایت Claude وارد بخش **Projects** شوید و یک پروژه جدید بسازید.
2. در قسمت **Set project instructions**، محتوای فایل [`core/UNIVERSAL_SYSTEM_PROMPT.md`](core/UNIVERSAL_SYSTEM_PROMPT.md) را پیست کنید.
3. قابلیت **Artifacts** را در تنظیمات اکانت خود روشن نگه دارید تا پرامپت نهایی دروازه ۴ در یک پنجره مجزا کامپایل شود.

**روش دوم (Claude Code CLI / Cursor):**
اگر از **Claude Code** در ترمینال یا **Cursor** استفاده میکنید، فایل [`platforms/claude/SKILL.md`](platforms/claude/SKILL.md) را در مسیر اسکیلهای خود کپی کنید:
```bash
mkdir -p ~/.claude/skills/idea-drill-through
cp platforms/claude/SKILL.md ~/.claude/skills/idea-drill-through/SKILL.md
```
سپس در هر پروژهای با تایپ `@idea-drill-through` یا `/idea-drill-through` اسکیل فعال میشود.

---

### ۳. نصب در Google Gemini (Gems & AI Studio)
1. در **Gemini Advanced** وارد بخش **Gem Manager -> New Gem** شوید (یا در **Google AI Studio** یک پرامپت جدید باز کنید).
2. نام Gem را `Idea Drill-Through` بگذارید.
3. محتوای فایل [`core/UNIVERSAL_SYSTEM_PROMPT.md`](core/UNIVERSAL_SYSTEM_PROMPT.md) را در کادر **Instructions (System Instructions)** کپی و ذخیره کنید.

---

## 🎮 چطور مکالمه را شروع کنیم؟

پس از نصب در هر یک از پلتفرمها، کافی است ایده یا مسئله خود را بنویسید یا فقط تایپ کنید:
> «میخوام فرآیند Idea Drill-Through رو برای یک تحلیل/ایده جدید شروع کنم.»

مدل بلافاصله **دروازه ۱** را باز کرده و با نمایش جدول امتیازدهی (Clarity Scorecard) شما را گامبهگام هدایت میکند.

---

## 📜 لایسنس
این پروژه تحت لایسنس **MIT** منتشر شده است. استفاده، فورک کردن و سفارشیسازی آن برای تیمهای محصول، دیتا و استراتژی کاملاً آزاد است.