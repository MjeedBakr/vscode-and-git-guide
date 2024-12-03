# إنشاء مشروع ورفعه على GitHub باستخدام VSCode

## الخطوة 1: تثبيت الأدوات الأساسية
1. قم بتثبيت **Git** على جهازك من [git-scm.com](https://git-scm.com/downloads/)
2. قم بتثبيت **Visual Studio Code** من [code.visualstudio.com](https://code.visualstudio.com/)
3. أنشئ حسابًا على **GitHub** إذا لم يكن لديك حساب

---

## الخطوة 2: إنشاء المشروع في VSCode
1. افتح VSCode واختر **File > Open Folder** لفتح مجلد مشروعك

---

## الخطوة 3: ربط المشروع بـ Git
1. افتح Terminal داخل VSCode من قائمة **Terminal > New Terminal**.
2. نفّذ الأوامر التالية:
   - تفعيل Git في المجلد:
     ```bash
     git init
     ```
   - إضافة جميع الملفات إلى المرحلة الأولى:
     ```bash
     git add .
     ```
   - حفظ أول تعديل:
     ```bash
     git commit -m "هنا اكتب الكومنت حقك"
     ```

---

## الخطوة 4: إنشاء repo على GitHub
1. اذهب إلى [GitHub](https://github.com/) وأنشئ repo جديد
2. اختر اسمًا للـ repo واضبط الخيارات (عام أو خاص)
3. انسخ رابط الـ repo

---

## الخطوة 5: ربط المشروع المحلي بمستودع GitHub
1. في Terminal داخل VSCode، استخدم الأوامر التالية:
   ```bash
   git remote add origin <رابط المشروع الي نسخته>
   git branch -M main
   git push -u origin main
