<!-- ELUCENIA technical documentation · qsofa · ar · no clinical/professional/rights approval -->

# qSOFA (SOFA السريع)

[الشروط والمصادر والأذونات](https://elucenia.org/ar/tools/qsofa)

## كيفية الاستخدام

استخدم الأداة في البوابة أو افتح index.html عبر خادم HTTP محلي. اختر اللغة، وأكمل الحقول، ثم أجرِ الحساب.

## المدخلات والوحدات

### معدل التنفس ≥ ٢٢ irpm

`fr`

### تغير الحالة الذهنية (Glasgow \< ١٥)

`mental`

### الضغط الانقباضي ≤ ١٠٠ mmHg

`pas`

## إصدار الطريقة

qSOFA/Sepsis-3/Seymour 2016: التنفس≥22/الانقباضي≤100/تغير الوعي، 0–3؛ SSC 2021 لا يوصي بالتحري المنفرد

## المعادلة الموثقة

نقطة لكل: التنفس ≥ 22/min، تغير الوعي، الانقباضي ≤ 100 mmHg. إيجابي عند 2 نقطة أو أكثر.

## الحدود والفئة السكانية

qSOFA2016 أداة لتقييم الخطر لدى البالغين المشتبه بإصابتهم بعدوى، وليس تشخيصًا ولا اختبارًا منفردًا لاستبعاد الإنتان. لا تنفي الدرجة المنخفضة الاشتباه السريري. توصي SSC2021 بعدم استخدام qSOFA بوصفه أداة التحري الوحيدة؛ وتظل إرشادات SSC2026 الرسمية تفضّل أدوات أخرى للتحري في المستشفى. يجب ألا ينتظر التقييم والعلاج الطارئ حسابَ المقياس. لا تثبت هذه العتبة الخاصة بالبالغين تطبيقًا لدى الأطفال.

## المراجع

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

## إعادة إجراء الاختبارات التقنية

شغّل node test.cjs في المجلد الجذري لهذا المستودع لتكرار الحالات الاصطناعية المسجلة. تُحفظ المدخلات والنتائج المتوقعة وحدود التفاوت الأصلية. لا تُعدّ الاختبارات التقنية تحققًا سريريًا.

```sh
node test.cjs
```

يحتوي tool.json على المصادر والإصدار ونطاق المراجعة. يحتفظ examples.json بالمدخلات والنتائج المتوقعة للحالات الاصطناعية؛ ويسجل results.json النتائج التي تم الحصول عليها.

[السجل والمراجع](../tool.json) · [شيفرة JavaScript](../calculator.js) · [حالات مرجعية](../examples.json) · [results.json](../results.json)

## المراجعة وشروط الاستخدام

لم تُجرَ مراجعة سريرية مستقلة.

هذه الواجهة ترجمة أعدّها مؤلفوها، وليست إصدارًا رسميًا أو معتمدًا. لم تُجرَ مراجعة سريرية مستقلة أو مراجعة لغوية مهنية، ولم تُستكمل الموافقة على حقوق استخدام الأدوات.

نتيجة المعادلة أو التصنيف. يعتمد التفسير والتصرف ومدى الانطباق على التقييم المهني والمصدر المحدد.

## الترخيص ونسبة العمل إلى أصحابه

ينطبق Apache-2.0 على كود ELUCENIA فقط. تبقى حقوق الأدوات والمنشورات والترجمات والبيانات لأصحابها المعنيين. احتفظ بملفّي LICENSE وNOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
