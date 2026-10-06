<!-- ELUCENIA technical documentation · qsofa · hi · no clinical/professional/rights approval -->

# qSOFA (त्वरित SOFA)

[शर्तें, स्रोत और अनुमतियाँ](https://elucenia.org/hi/tools/qsofa)

## उपयोग कैसे करें

पोर्टल पर उपकरण का उपयोग करें या स्थानीय HTTP सर्वर के माध्यम से index.html खोलें। भाषा चुनें, फ़ील्ड भरें और गणना करें।

## इनपुट और इकाइयाँ

### श्वसन दर ≥ 22 irpm

`fr`

### मानसिक स्थिति में बदलाव (Glasgow \< 15)

`mental`

### सिस्टोलिक दबाव ≤ 100 mmHg

`pas`

## विधि का संस्करण

qSOFA/Sepsis-3/Seymour 2016: श्वसन≥22/सिस्टोलिक≤100/मानसिक परिवर्तन, 0–3; SSC 2021 अकेली स्क्रीनिंग अनुशंसित नहीं

## दस्तावेज़ित सूत्र

हर एक का एक अंक: श्वसन ≥ 22/min, मानसिक स्थिति परिवर्तन, सिस्टोलिक ≤ 100 mmHg। 2 या अधिक अंक पर सकारात्मक।

## सीमाएँ और जनसमूह

qSOFA2016 संदिग्ध संक्रमण वाले वयस्कों में जोखिम का आकलन करने का साधन है; यह न तो निदान है और न ही सेप्सिस को खारिज करने वाला अकेला परीक्षण। कम स्कोर नैदानिक संदेह समाप्त नहीं करता। SSC2021, qSOFA को एकमात्र स्क्रीनिंग साधन के रूप में उपयोग करने के विरुद्ध सिफारिश करता है; आधिकारिक SSC2026 मार्गदर्शन भी अस्पताल में स्क्रीनिंग के लिए अन्य साधनों को प्राथमिकता देता है। आपातकालीन आकलन और उपचार को स्कोर की प्रतीक्षा में नहीं रोकना चाहिए। वयस्कों की यह सीमा बच्चों में उपयोग स्थापित नहीं करती.

## संदर्भ

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

## तकनीकी परीक्षण दोहराएँ

दर्ज कृत्रिम मामलों को दोहराने के लिए इस रिपॉज़िटरी की मूल निर्देशिका में node test.cjs चलाएँ। मूल इनपुट, अपेक्षित परिणाम और सहनशीलता सीमाएँ सुरक्षित रखी गई हैं। तकनीकी परीक्षण नैदानिक सत्यापन नहीं हैं।

```sh
node test.cjs
```

tool.json में स्रोत, संस्करण और समीक्षा का दायरा दिया गया है। examples.json में कृत्रिम इनपुट और अपेक्षित परिणाम सुरक्षित हैं; results.json में प्राप्त परिणाम दर्ज हैं।

[रिकॉर्ड और संदर्भ](../tool.json) · [JavaScript कोड](../calculator.js) · [संदर्भ मामले](../examples.json) · [results.json](../results.json)

## समीक्षा और उपयोग की शर्तें

स्वतंत्र नैदानिक समीक्षा नहीं की गई है।

यह इंटरफ़ेस लेखकों द्वारा किया गया अनुवाद है, कोई आधिकारिक या प्रमाणित संस्करण नहीं। स्वतंत्र नैदानिक समीक्षा, पेशेवर भाषाई समीक्षा और उपकरणों के अधिकारों की अनुमति की प्रक्रिया पूरी नहीं हुई है।

सूत्र या वर्गीकरण का परिणाम। व्याख्या, कार्यवाही और उपयुक्तता पेशेवर मूल्यांकन और चुने गए स्रोत पर निर्भर है।

## लाइसेंस और श्रेय

Apache-2.0 केवल ELUCENIA के कोड पर लागू होता है। उपकरणों, प्रकाशनों, अनुवादों और डेटा के अधिकार उनके संबंधित अधिकारधारकों के पास रहते हैं। LICENSE और NOTICE सुरक्षित रखें।

ELUCENIA · Felipe Guedes · Copyright © 2026

## दर्ज किए गए परिणाम

नीचे दी गई जानकारी कृत्रिम उदाहरणों के लिए पद्धति के आउटपुट को सुरक्षित रखती है। यह स्वतंत्र नैदानिक सत्यापन नहीं है।

### 1

qSOFA नकारात्मक (< 2)

सेप्सिस को बाहर नहीं करता: पुनर्मूल्यांकन जारी रखें और यदि अंग विकृति का संदेह हो तो SOFA की गणना करें।


### 2

qSOFA सकारात्मक (≥ 2): अस्पताल में मृत्यु का अधिक जोखिम

अंग विकृति (SOFA) की जांच करें, सेप्सिस बंडल शुरू करें और ICU पर विचार करें।


### 3

qSOFA सकारात्मक (≥ 2): अस्पताल में मृत्यु का अधिक जोखिम

अंग विकृति (SOFA) की जांच करें, सेप्सिस बंडल शुरू करें और ICU पर विचार करें।

