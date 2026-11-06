# Employee Exam System

نظام اختبارات إلكتروني للموظفين — صفحة واحدة (index.html) متصلة بقاعدة بيانات Firebase.

## النشر على GitHub ثم Vercel

1. ارفعي محتوى هذا المجلد كـ repository جديد على GitHub (أنشئي repo فارغ، ثم:
   ```
   git init
   git add .
   git commit -m "Employee Exam System"
   git branch -M main
   git remote add origin <رابط الـ repo بتاعك>
   git push -u origin main
   ```
   أو ارفعي الملفات مباشرة من واجهة GitHub (Add file → Upload files) من غير أوامر.

2. على vercel.com: سجّلي دخول (بإيميلك أو حساب GitHub) → New Project →
   اختاري الـ repo ده → اضغطي Deploy. لا يوجد Build Command مطلوب (موقع ثابت).

3. هتاخدي رابط فورًا زي: `your-project.vercel.app` — يشتغل من أي متصفح وأي جهاز
   بدون أي علاقة بـ Claude، ويحفظ البيانات في Firebase الخاص بيك مباشرة.

## قبل النشر — تأكدي من:
- فعّلتي Firestore Database في مشروع Firebase.
- ضبطتي Rules في Firestore (allow read, write: if true؛ أو قواعد أكثر أمانًا لاحقًا).
- كلمة مرور المدير الافتراضية: 8520 (تقدري تغيّريها من صفحة الإعدادات داخل النظام).
