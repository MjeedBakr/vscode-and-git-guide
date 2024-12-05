# إنشاء مشروع ورفعه على GitHub باستخدام VSCode

## الخطوة 0: تثبيت الأدوات الأساسية
1. قم بتثبيت **Git** على جهازك من [git-scm.com](https://git-scm.com/downloads/)
2. قم بتثبيت **Visual Studio Code** من [code.visualstudio.com](https://code.visualstudio.com/)
3. أنشئ حسابًا على **GitHub** إذا لم يكن لديك حساب



## الخطوة 1: إنشاء المشروع في VSCode
1. افتح VSCode واختر **File > Open Folder** لفتح مجلد مشروعك



## الخطوة 2: ربط المشروع بـ Git
1. افتح Terminal داخل VSCode من قائمة **Terminal > New Terminal**
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



## الخطوة 3: إنشاء repo على GitHub
1. اذهب إلى [GitHub](https://github.com/) وأنشئ repo جديد
2. اختر اسمًا للـ repo واضبط الخيارات (عام أو خاص)
3. انسخ رابط الـ repo



## الخطوة 4: ربط المشروع المحلي بـ ريبو GitHub
1. في Terminal داخل VSCode، استخدم الأوامر التالية:
   - يستخدم هذا الأمر لإضافة repo بعيد (الي على Github) وربطه بالـ repo المحلي (الي على جهازك):
     ```bash
     git remote add origin رابط المشروع الي نسخته
     ```
   - يتغيير اسم الـ branch الحالي إلى main:
     ```bash
     git branch -M main
     ```
   - رفع التعديلات الموجودة على الـ branch من الـ repo المحلي إلى الـ repo البعيد:
     ```bash
     git push origin main
     ```


---
# **طريقة العمل على المشروع**  
   - إضافة جميع الملفات إلى المرحلة الأولى (أو ملف معين زي في السطر الثاني):
     ```bash
     git add .
     git add اسم الملف
     ```
   - حفظ التعديلات:
     ```bash
     git commit -m "هنا اكتب الكومنت حقك"
     ```
   - رفع التعديلات الموجودة على الـ branch من الـ repo المحلي إلى الـ repo البعيد:
     ```bash
     git push origin main
     ```
---




---
