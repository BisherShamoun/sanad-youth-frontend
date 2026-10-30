# Sanad Youth Frontend - منصة سند الشباب

واجهة أماميّة متكاملة تم بناؤها باستخدام **React**, **Vite**, **Tailwind CSS**, و **React Router** لربطها بباك إند **Sanad Youth (NestJS)**.

## 🚀 المميزات والصفحات

1. **المصادقة (Auth)**:
   - تسجيل الدخول (`/login`) وتسجيل شاب جديد (`/register`).
   - حفظ JWT Token وربطه تلقائياً مع Axios Interceptors.
2. **البرامج التدريبية (Programs)**:
   - استعراض البرامج التدريبية مع البحث والصفحات (`/programs`).
   - تفاصيل البرنامج والتقديم المباشر ورفع السيرة الذاتية CV (`/programs/:id`).
   - إنشاء برنامج جديد للمشرفين والمسؤولين (`/programs/create`).
3. **الجلسات والمواد (Sessions & Materials)**:
   - إضافة جلسات تدريبية للبرنامج.
   - رفع وتنزيل المواد المرفقة بالكورس.
4. **الطلبات (Applications)**:
   - مراجعة طلباتي الشخصية وإلغاؤها (`/my-applications`).
   - مراجعة طلبات المتقدمين وقبولها/رفضها من قبل المشرفين.
5. **الإعلانات (Announcements)**:
   - استعراض وإضافة إعلانات عامة أو خاصة ببرامج معينة (`/announcements`).
6. **إدارة المشرفين (Supervisors Management)**:
   - إنشاء حسابات مشرفين من قبل Admin (`/admin/supervisors`).

## 🛠️ كيفية التشغيل

1. فك الضغط عن الملف:
   ```bash
   unzip sanad-youth-frontend.zip
   cd sanad-youth-frontend
   ```
2. تثبيت الحزم والمكتبات:
   ```bash
   npm install
   ```
3. تشغيل سيرفر التطوير المحلي (Dev Server):
   ```bash
   npm run dev
   ```
   سيعمل المشروع على: `http://localhost:5173`

4. ربط الـ API:
   - يتصل التطبيق افتراضياً بـ `http://localhost:3000/api`.
   - يمكنك تغيير الرابط عن طريق إنشاء ملف `.env`:
     ```env
     VITE_API_URL=http://localhost:3000/api
     ```
