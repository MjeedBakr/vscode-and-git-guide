# إنشاء مشروع ورفعه على GitHub باستخدام VSCode

## الخطوة 1: تثبيت الأدوات الأساسية
1. قم بتثبيت **Git** على جهازك من [git-scm.com](https://git-scm.com/downloads/)
2. قم بتثبيت **Visual Studio Code** من [code.visualstudio.com](https://code.visualstudio.com/)
3. أنشئ حسابًا على **GitHub** إذا لم يكن لديك حساب



## الخطوة 2: إنشاء المشروع في VSCode
1. افتح VSCode واختر **File > Open Folder** لفتح مجلد مشروعك



## الخطوة 3: ربط المشروع بـ Git
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



## الخطوة 4: إنشاء repo على GitHub
1. اذهب إلى [GitHub](https://github.com/) وأنشئ repo جديد
2. اختر اسمًا للـ repo واضبط الخيارات (عام أو خاص)
3. انسخ رابط الـ repo



## الخطوة 5: ربط المشروع المحلي بـ ريبو GitHub
1. في Terminal داخل VSCode، استخدم الأوامر التالية:
   ```bash
   git remote add origin رابط المشروع الي نسخته
   git branch -M main
   git push origin main
   ```

---


# **استنساخ الـ repo للمشارك الجديد**  

بعد إرسال الدعوة، يجب على الشخص الجديد اتباع الخطوات التالية:

1. انسخ رابط الـ repo
2. افتح **Terminal** أو **VSCode**
5. قم بتشغيل الأمر التالي:
   ```bash
   git clone رابط المشروع الي نسخته
   ```
   على سبيل المثال:
   ```bash
   git clone https://github.com/username/repository-name.git
   ```




---



# آلية العمل مع فريق باستخدام Branches

## الخطوة 1: إنشاء Branch جديد

1. تأكد أنك على الـ branch الرئيسي `main`
   ```bash
   git checkout main
   git pull origin main
   ```
2. قم بإنشاء branch جديد للعمل عليه:
   ```bash
   git branch اسم_البرانش
   git checkout اسم_البرانش
   ```




## الخطوة 2: العمل على الـ branch

1. قم بإجراء التعديلات أو إضافة المميزات على المشروع
2. بعد الانتهاء من التعديلات، احفظ التغييرات
   ```bash
   git add .
   git commit -m "وصف للتعديلات التي أجريتها"
   ```



## الخطوة 3: رفع الbranch إلى GitHub

1. بعد حفظ التعديلات في الـ branch، قم برفعه إلى GitHub
   ```bash
   git push origin اسم_البرانش
    مو main!!!
   ```



## الخطوة 4: إنشاء Pull Request على GitHub

1. بعد رفع الـ branch إلى GitHub، قم بإنشاء **Pull Request** لدمج التعديلات إلى الـ branch الرئيسي
2. انتقل إلى صفحة الـ repo على GitHub
3. اضغط على "Compare & Pull Request"، ثم أضف وصفًا للتعديلات التي أجريتها
4. انتظر موافقة أعضاء الفريق على التعديلات قبل دمجها



## الخطوة 5: دمج الـ branch إلى الـ branch الرئيسي

1. بعد أن يتم مراجعة التعديلات والموافقة عليها، قم بدمج الـ branch إلى `main`
2. اضغط على "Merge Pull Request" لإتمام الدمج



## الخطوة 6: حذف الـ branch بعد الدمج

1. بعد دمج التعديلات في `main`, يمكنك حذف الbranch من GitHub
2. في المشروع المحلي، قم بالتبديل إلى الbranch الرئيسي `main` ثم احذف الbranch محليًا
   ```bash
   git checkout main
   git branch -d اسم_البرانش
   ```



## الخطوة 7: تحديث المشروع المحلي

1. بعد دمج التعديلات في الbranch الرئيسي `main`، تأكد من مزامنة التعديلات في مشروعك المحلي
   ```bash
   git checkout main
   git pull origin main
   ```

---
