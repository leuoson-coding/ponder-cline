# المساهمة في Ponder

نحن سعداء لاهتمامك بالمساهمة في Ponder. سواء كنت تصلح خطأً أو تضيف ميزة أو تحسن الوثائق لدينا، فإن كل مساهمة تجعل Ponder أذكى! للحفاظ على مجتمعنا نابضًا بالحياة وترحيبيًا، يجب على جميع الأعضاء الالتزام بـ [مدونة قواعد السلوك](CODE_OF_CONDUCT.md) لدينا.

## الإبلاغ عن الأخطاء أو المشكلات

تساعد تقارير الأخطاء على جعل Ponder أفضل للجميع! قبل إنشاء مشكلة جديدة، يرجى [البحث عن المشكلات الموجودة](https://github.com/leuoson/ponder/issues) لتجنب الازدواجية. عندما تكون جاهزًا للإبلاغ عن خطأ، انتقل إلى [صفحة المشكلات](https://github.com/leuoson/ponder/issues/new/choose) حيث ستجد قالبًا لمساعدتك في ملء المعلومات ذات الصلة.

<blockquote class='warning-note'>
     🔐 <b>مهم:</b> إذا اكتشفت ثغرة أمنية، فيرجى استخدام <a href="https://github.com/leuoson/ponder/security/advisories/new">أداة الأمان على Github للإبلاغ عنها بشكل خاص</a>.
</blockquote>

## تحديد ما يجب العمل عليه

تبحث عن مساهمة أولى جيدة؟ تحقق من المشكلات المميزة بـ ["good first issue"](https://github.com/leuoson/ponder/labels/good%20first%20issue) أو ["help wanted"](https://github.com/leuoson/ponder/labels/help%20wanted). تم تحديد هذه المشكلات خصيصًا للمساهمين الجدد والمجالات التي نرحب فيها بالمساعدة!

نرحب أيضًا بالمساهمات في [الوثائق](https://github.com/leuoson/ponder/tree/main/docs) لدينا! سواء كان تصحيح أخطاء إملائية، أو تحسين الأدلة الحالية، أو إنشاء محتوى تعليمي جديد - نود بناء مستودع موارد مدفوع من المجتمع يساعد الجميع على الاستفادة القصوى من Ponder. يمكنك البدء بالغوص في `/docs` والبحث عن مجالات تحتاج إلى تحسين.

إذا كنت تخطط للعمل على ميزة أكبر، فيرجى إنشاء [طلب ميزة](https://github.com/leuoson/ponder/discussions/categories/feature-requests?discussions_q=is%3Aopen+category%3A%22Feature+Requests%22+sort%3Atop) أولاً حتى نتمكن من مناقشة ما إذا كان ذلك يتماشى مع رؤية Ponder.

## إعداد التطوير

1. **إضافات VS Code**

    - عند فتح المشروع، سيطالبك VS Code بتثبيت الإضافات الموصى بها
    - هذه الإضافات مطلوبة للتطوير - يرجى قبول جميع مطالبات التثبيت
    - إذا تجاهلت المطالبات، يمكنك تثبيتها يدويًا من لوحة الإضافات

2. **التطوير المحلي**
    - قم بتشغيل `npm run install:all` لتثبيت التبعيات
    - قم بتشغيل `npm run test` لتشغيل الاختبارات محليًا
    - قبل تقديم طلب السحب، قم بتشغيل `npm run format:fix` لتنسيق التعليمات البرمجية الخاصة بك

## كتابة وتقديم التعليمات البرمجية

يمكن لأي شخص المساهمة بالتعليمات البرمجية في Ponder، لكننا نطلب منك اتباع هذه الإرشادات لضمان دمج مساهماتك بسلاسة:

1. **احتفظ بطلبات السحب مركزة**

    - قيد طلبات السحب بميزة واحدة أو إصلاح خطأ
    - قسم التغييرات الأكبر إلى طلبات سحب أصغر ومتصلة
    - قسم التغييرات إلى التزامات منطقية يمكن مراجعتها بشكل مستقل

2. **جودة التعليمات البرمجية**

    - قم بتشغيل `npm run lint` للتحقق من نمط التعليمات البرمجية
    - قم بتشغيل `npm run format` لتنسيق التعليمات البرمجية تلقائيًا
    - يجب أن تجتاز جميع طلبات السحب عمليات التحقق المستمر التي تشمل كلاً من التنضيد والتنسيق
    - تعامل مع أي تحذيرات أو أخطاء ESLint قبل التقديم
    - اتبع أفضل ممارسات TypeScript والحفاظ على سلامة النوع

3. **الاختبار**

    - أضف اختبارات للميزات الجديدة
    - قم بتشغيل `npm test` للتأكد من اجتياز جميع الاختبارات
    - قم بتحديث الاختبارات الحالية إذا كانت تغييراتك تؤثر عليها
    - تضمين كل من اختبارات الوحدة واختبارات التكامل حيثما كان ذلك مناسبًا

4. **إدارة الإصدار مع Changesets**

    - أنشئ changeset لأي تغييرات واجهة المستخدم باستخدام `npm run changeset`
    - اختر زيادة الإصدار المناسبة:
        - `major` للتغييرات الكبيرة (1.0.0 → 2.0.0)
        - `minor` للميزات الجديدة (1.0.0 → 1.1.0)
        - `patch` لإصلاحات الأخطاء (1.0.0 → 1.0.1)
    - اكتب رسائل changeset واضحة ووصفية تشرح التأثير
    - لا تتطلب التغييرات في الوثائق فقط changesets

5. **إرشادات الالتزام (Commit Guidelines)**

   - اكتب رسائل التزام واضحة وواصفة  
   - استخدم تنسيق الالتزام التقليدي (مثل: "feat:", "fix:", "docs:")  
   - أشر إلى القضايا ذات الصلة في الالتزامات باستخدام #رقم-القضية  

6. **قبل الإرسال**

   - قم بإعادة دمج فرعك مع أحدث إصدار من الفرع الرئيسي  
   - تأكد من أن الفرع الخاص بك يُبنى بنجاح  
   - تحقق من اجتياز جميع الاختبارات  
   - راجع التغييرات الخاصة بك للتأكد من عدم وجود تعليمات تصحيح الأخطاء أو سجلات وحدة التحكم  

7. **وصف طلب السحب (Pull Request Description)**

   - صف بوضوح ما تقوم به التغييرات  
   - قم بتضمين خطوات لاختبار التغييرات  
   - أدرج أي تغييرات غير متوافقة  
   - أضف لقطات شاشة للتغييرات في واجهة المستخدم  

## اتفاقية المساهمة  

من خلال إرسال طلب سحب، فإنك توافق على أن مساهماتك سيتم ترخيصها بنفس ترخيص المشروع ([Apache 2.0](LICENSE)).  

تذكر: المساهمة في Ponder لا تقتصر فقط على كتابة الكود - إنها تتعلق بأن تكون جزءًا من مجتمع يُشكل مستقبل التطوير بمساعدة الذكاء الاصطناعي. لنبنِ شيئًا رائعًا معًا! 🚀