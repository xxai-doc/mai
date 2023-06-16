<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.कला के अनुसार

वेबसाइट कोड केरऽ एगो हिस्सा ओपन सोर्स छै, अनुवाद क॑ अनुकूलित करै म॑ मदद करै लेली स्वागत छै ।

## फ्रंट-एंड कोड

* [फ्रंट-एंड कोड](https://github.com/xxai-art/web)
* [समग्र रूप स साइट क लेल भाषा पैक](https://github.com/xxai-art/web/tree/main/i18n)
* [लॉगिन मॉड्यूल क लेल भाषा पैक](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [वेबसाइट बहुभाषी दस्तावेजीकरण](https://github.com/xxai-doc)

फ्रंट-एंड प्रोग्रामिंग भाषा [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) अछि, जे कॉफीस्क्रिप्ट सिंटैक्स के आधार पर किछु सुविधा जोड़ैत अछि, देखू [./coffee_plus.md](./coffee_plus.md) .

## वेबसाइट एवं दस्तावेज के अंतर्राष्ट्रीयकरण

निम्नलिखित 3 परियोजना पर निर्माण करू

* [@ w5/mdt पर](https://www.npmjs.com/package/@w5/mdt)

  प्रत्यय `.mdt` अछि , अहाँ बाहरी फाइल केँ संदर्भित करबाक लेल `<+ ./coffee_plus/import.js>` क' समान वाक्य रचना क' उपयोग क' सकैत छी, आओर `.md` प्रत्यय क' संग मार्कडाउन उत्पन्न क' सकैत छी.

* [@ w5/trmd पर](https://www.npmjs.com/package/@w5/trmd)

  मार्कडाउन अनुवाद कोड आ लिंक के अनुवाद नै करत, आ अनुवादित वाक्य के कैश करत. यदि अनुवाद में संशोधन करलऽ गेलऽ छै लेकिन मूल पाठ में संशोधन नै करलऽ गेलऽ छै त॑ ओकरा दोबारा निष्पादित करला स॑ अनुवाद के संशोधन क॑ ओवरराइट नै करलऽ जैतै ।

* [@ w5/i18n पर](https://www.npmjs.com/package/@w5/i18n)

  `yaml` उत्पन्न वेबसाइट के अनुवाद के लिये भाषा फाइल |
