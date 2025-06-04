# 📘 Maham School Management System

A full-featured school management system built with React, supporting both public-facing website and internal dashboards for administrators, students, teachers, and parents. Designed with multilingual support (English/Arabic) and full RTL support for Arabic UI.

---

## 🌐 Live Preview

Coming Soon...

---

## 📂 Project Structure

```bash
maham-school/
│
├── External-site/           # الموقع الخارجي (React, Angular...)
├── mobile-app/              # تطبيق الموبايل (React Native, Flutter...)
├── api/                     # API (ASP.NET Core, Node.js...)
├── database/                # سكربتات إنشاء قاعدة البيانات / البيانات الأولية
├── docs/                    # وثائق المشروع
└── README.md


🚀 Features
🌍 Public Website
School introduction and news

Programs and events

Contact form with map

Fully responsive

RTL + Multilingual (EN/AR)

🛠️ Admin Dashboard
Student management

Teacher & class schedules

Attendance & grades

Role-based login (Admin / Teacher / Student / Parent)

Notifications and calendar

🧑‍💻 Tech Stack
React.js + React Router

Redux Toolkit or Context API

React-i18next for internationalization

Bootstrap 5 / Tailwind CSS

RTL support via CSS & plugins

Axios for API requests

Node.js / Express / Firebase / Supabase (optional backend)


## 💡 لماذا اخترنا هذه الخدمات؟

نهدف إلى بناء نظام قوي ومرن، لذلك اخترنا كل خدمة حسب تخصصها:

| الخدمة | السبب |
|--------|--------|
| **Vercel** | لاستضافة الواجهة الخارجية المبنية بـ React – يدعم نشر تلقائي، CDN، وأداء عالي. |
| **MongoDB Atlas / Supabase** | لإدارة البيانات – سهلة الاستخدام، تدعم API مباشر، وتحكم قوي في البيانات. |
| **Postmark / Brevo** | لإرسال الإشعارات عبر البريد الإلكتروني – موثوقة وسريعة واحترافية. |

كل خدمة مصممة لتؤدي وظيفة معينة بكفاءة، ودمجهم معًا يعطينا بنية نظيفة وقابلة للتوسع.

---

## 🔗 كيف يتواصل النظام الداخلي؟ (Architecture Overview)

### 🧩 المكونات:

- **Frontend (React)**: يتم استضافته على Vercel – يتفاعل مع API لعرض البيانات.
- **Mobile App (Flutter)**: يتفاعل أيضًا مع نفس الـ API للحصول على البيانات من نفس المصدر.
- **Backend API (Node.js / Next.js)**: هو الوسيط بين الواجهات المختلفة وقاعدة البيانات وخدمة البريد.
- **Database (MongoDB أو Supabase)**: لتخزين بيانات المستخدمين والمدارس والطلاب وكل ما يتعلق بالنظام.
- **Email Service (Postmark / Brevo)**: لإرسال رسائل التأكيد والتنبيهات والإشعارات.

### 🔁 مثال تدفق البيانات:
1. يسجل المستخدم حسابًا.
2. ترسل الواجهة بيانات التسجيل إلى الـ API.
3. يتحقق الـ API من البيانات ويخزنها في قاعدة البيانات.
4. يرسل الـ API بريدًا إلكترونيًا لتأكيد التسجيل عبر Postmark.
5. يتلقى المستخدم رسالة تأكيد على بريده الإلكتروني.

