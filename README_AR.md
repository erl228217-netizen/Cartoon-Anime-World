# CARTOON & ANIME WORLD — حزمة GitHub Pages

هذه هي النسخة النهائية الجاهزة للرفع إلى مستودع باسم `cartoon-anime-world`. حافظت الحزمة على الواجهة الأصلية وتضم `index.html` في الجذر، وملفات JavaScript وFirebase وقواعد Firestore والتوثيق. الصور الموجودة في الواجهة مضمّنة داخل `index.html`، لذلك لا توجد مجلدات صور ناقصة.

## التشغيل المحلي

```bash
python3 -m http.server 4173
```

افتح `http://localhost:4173/`. لا تفتح `index.html` مباشرة لأن Firebase وES Modules يحتاجان خادم HTTP.

## الرفع إلى GitHub Pages

1. أنشئ مستودعًا عامًا باسم `cartoon-anime-world`.
2. ارفع **محتويات هذه الحزمة بعد فك الضغط** إلى الجذر، بحيث يكون المسار `cartoon-anime-world/index.html`.
3. من `Settings > Pages` اختر `Deploy from a branch`، ثم فرع `main` والمجلد `/ (root)`.
4. احفظ وانتظر رابط GitHub Pages. جميع مسارات الموقع نسبية، وملف `.nojekyll` مرفق.

## Firebase

`firebase-config.js` يحتوي قيمًا placeholder عمدًا، ولا توجد مفاتيح سرية داخل الحزمة. لاستعمال تسجيل البريد وGoogle واستعادة كلمة المرور وFirestore، ضع إعدادات Web App الخاصة بك، فعّل المزودين، وأضف نطاق GitHub Pages إلى Authorized domains. استبدل بريد المدير في `firebase-config.js` و`firestore.rules` قبل النشر.

## الحالة

الواجهة والبحث والمفضلة وسجل المشاهدة والتنقل واختبار الهاتف تعمل محليًا. تسجيل الدخول الحقيقي، Google، إرسال رابط استعادة كلمة المرور، وعمليات لوحة الإدارة الحقيقية تحتاج إعداد Firebase؛ لا تعتبر مفعلة قبل ذلك. الدفع والفيديوهات المحمية غير مفعّلين.
