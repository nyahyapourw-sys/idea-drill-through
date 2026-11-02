# راهنمای استفاده در Google Gemini Gems و Google AI Studio

این راهنما برای راه‌اندازی **Idea Drill-Through (AI Checklist Architect)** در سرویس‌های **Gemini Gems (Gemini Advanced)** و **Google AI Studio** آماده شده است.

---

## 🔹 روش ۱: راه‌اندازی در Google Gemini Gems (کاربران Gemini Advanced / Workspace)

1. به [gemini.google.com](https://gemini.google.com) بروید.
2. در منوی سمت چپ، روی **Gem Manager** و سپس **New Gem** کلیک کنید.
3. مشخصات Gem را به شرح زیر تنظیم کنید:
   - **Name:** `Idea Drill-Through (AI Checklist Architect)`
   - **Instructions:** محتوای فایل `core/UNIVERSAL_SYSTEM_PROMPT.md` را کپی و در کادر دستورالعمل وارد کنید.
4. روی **Save** کلیک کنید.
5. اکنون می‌توانید در هر گفتگویی این Gem را انتخاب کرده و فرآیند ۵ دروازه‌ای را اجرا نمایید.

---

## 🔹 روش ۲: راه‌اندازی در Google AI Studio (توسعه‌دهندگان و مهندسان پرامپت)

1. وارد [aistudio.google.com](https://aistudio.google.com) شوید.
2. یک **New Chat Prompt** یا **New Structured Prompt** ایجاد کنید.
3. مدل پیشنهادی را روی **Gemini 2.5 Flash** یا **Gemini 2.5 Pro** قرار دهید.
4. در بخش **System Instructions**، متن فایل `core/UNIVERSAL_SYSTEM_PROMPT.md` را وارد کنید.
5. پارامترهای مدل:
   - **Temperature:** `0.2` تا `0.4` (جهت حفظ دقت دترمینیستیک و جلوگیری از توهم اعداد)
   - **Top-P:** `0.9`
6. پرامپت را ذخیره کرده و به عنوان یک ابزار مهندسی پرامپت تیمی استفاده کنید.