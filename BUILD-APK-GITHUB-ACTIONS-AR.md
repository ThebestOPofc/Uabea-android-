# بناء UABEA Android APK عبر GitHub Actions

هذا المستودع يتضمن سير العمل `.github/workflows/build-android-apk.yml`.

## ماذا ينتج؟
- يبني مشروع `UABEA.Android.Android` باستخدام .NET 8 وAndroid workload.
- ينتج APK من نوع Debug وموقّعاً بمفتاح Android debug الافتراضي.
- يرفع الملف كـ Artifact باسم `UABEA-Android-English-debug-APK`.

## التشغيل من الهاتف
1. أنشئ مستودعاً جديداً على GitHub وارفع إليه **محتويات هذا المجلد بعد فك الضغط**، وليس ملف ZIP نفسه.
2. تأكد أن ملف workflow موجود في المسار `.github/workflows/build-android-apk.yml`.
3. افتح تبويب Actions في المستودع.
4. اختر `Build UABEA Android APK` ثم `Run workflow`، أو انتظر تشغيله تلقائياً بعد أول push إلى `main` أو `master`.
5. افتح عملية التشغيل وانتظر علامة النجاح الخضراء.
6. من قسم Artifacts في أسفل صفحة التشغيل نزّل `UABEA-Android-English-debug-APK`.
7. فك ضغط ملف Artifact ثم ثبّت APK على هاتف Android.

## ملاحظات
- هذه نسخة Debug للتجربة، وموقّعة بمفتاح debug. ليست إصداراً نهائياً للنشر.
- إذا كان لديك إصدار آخر من التطبيق مثبتاً وموقّعاً بمفتاح مختلف، قد تحتاج إلى إزالته قبل تثبيت هذه النسخة.
- إذا فشل البناء، افتح سجل خطوة Build وانسخ رسالة الخطأ كاملة.
- لا ترفع أي keystore أو كلمات مرور توقيع إلى المستودع.
