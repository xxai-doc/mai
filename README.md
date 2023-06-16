<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

अनुशंसित अछि जे पहिने nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) इंस्टॉल करू, आओर फेर `direnv allow` निर्देशिका मे प्रवेश करबाक बाद ( डायरेक्टरी मे प्रवेश करबाक बाद [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वचालित रूप सँ निष्पादित भ' जाएत).

अर्थ है: चीनी अनुवाद जापानी, कोरियाई, अंग्रेजी, अन्य सभी भाषाओं में अंग्रेजी अनुवाद | अगर अहां केवल चीनी आ अंग्रेजी के समर्थन करय चाहय छी तं बस `zh: en` लिखि सकय छी.

अर्थ है: चीनी अनुवाद जापानी, कोरियाई, अंग्रेजी, अन्य सभी भाषाओं में अंग्रेजी अनुवाद | अगर अहां केवल चीनी आ अंग्रेजी के समर्थन करय चाहय छी तं बस `zh: en` लिखि सकय छी.

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

### दस्तावेज अनुवाद स्वचालन निर्देश

कोड भंडार [xxai-art/doc](https://github.com/xxai-art/doc) देखू

अनुशंसित अछि जे पहिने nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) इंस्टॉल करू, आओर फेर `direnv allow` निर्देशिका मे प्रवेश करबाक बाद ( डायरेक्टरी मे प्रवेश करबाक बाद [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वचालित रूप सँ निष्पादित भ' जाएत).

सैकड़ों भाषा मे अनुवादित पैघ कोड बेस स बचबाक लेल हम प्रत्येक भाषा क लेल अलग कोड बेस बनेलहुं आ कोड बेस कए स्टोर करबा लेल एकटा संगठन बनेलहुं

वातावरण चर `GITHUB_ACCESS_TOKEN` सेट करनाय आओर ओकर बाद [create.github.coffee कें](https://github.com/xxai-art/doc/blob/main/create.github.coffee) चलानाय स्वचालित रूप सं कोड भंडार बनायत.

ओना त अहां एकरा कोड बेस मे सेहो राखि सकय छी.

अनुवाद स्क्रिप्ट संदर्भ [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

स्क्रिप्ट कोड कें व्याख्या निम्नलिखित छै:

[bunx](https://bun.sh/docs/cli/bunx) npx क' प्रतिस्थापन अछि, जे तेज अछि. ओना त' जँ अहाँ लग बन इंस्टॉल नहि अछि त' एकर बदला मे `npx` प्रयोग क' सकैत छी.

`bunx mdt zh` zh निर्देशिका मे `.mdt` `.md` क' रूप मे प्रस्तुत करैत अछि, नीचाँ 2 लिंक कएल गेल फाइल देखू

* [कॉफी_प्लस.एमडीटी](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [कॉफी_प्लस.एमडी](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` अनुवाद क लेल कोर कोड अछि (जँ अहाँक पास केवल `nodejs` इंस्टॉल अछि, मुदा `bun` आ `direnv` इंस्टॉल नहि अछि, तँ अहाँ अनुवाद करबाक लेल `npx i18n` सेहो चला सकैत छी) ।

इ [i18n.yml कें](https://github.com/xxai-art/doc/blob/main/i18n.yml) पार्स करतय , अइ दस्तावेज मे `i18n.yml` कें विन्यास निम्नलिखित छै:

```
en:
zh: ja ko en
```

अर्थ है: चीनी अनुवाद जापानी, कोरियाई, अंग्रेजी, अन्य सभी भाषाओं में अंग्रेजी अनुवाद | अगर अहां केवल चीनी आ अंग्रेजी के समर्थन करय चाहय छी तं बस `zh: en` लिखि सकय छी.

अंतिम अछि [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , जे प्रत्येक भाषाक `README.md` के मुख्य शीर्षक आ पहिल उपशीर्षक के बीच सामग्री निकालैत अछि जे एकटा प्रविष्टि `README.md` उत्पन्न करैत अछि. कोड बहुत सरल अछि, अहां खुद देख सकय छी.

गूगल एपीआई के उपयोग मुफ्त अनुवाद के लेल कएल जाइत अछि. यदि अहां गूगल कें एक्सेस नहि कयर सकय छी, त कृपया एकटा प्रॉक्सी कॉन्फ़िगर आ सेट करू, जेना:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

अनुवाद स्क्रिप्ट `.i18n` निर्देशिका मे एकटा अनुवादित कैश उत्पन्न करत, कृपया एकरा `git status` क संग जाँच करू आओर एकरा कोड भंडार मे जोड़ू ताकि दोहराओल गेल अनुवाद स बचल जा सकय.

कृपया हर बेर जखन अहाँ कैश अपडेट करबाक लेल अनुवाद संशोधित करैत छी तखन `bunx i18n` चलाउ.

यदि मूल पाठ आरू अनुवाद एक साथ संशोधित करलऽ जाय छै, त॑ कैश भ्रमित होय जैतै, ई लेली अगर आप संशोधित करना चाहै छियै त॑ आप केवल एक क॑ संशोधित करी सकै छियै, आरू ओकरा बाद कैश क॑ अपडेट करै लेली `bunx i18n` चलाबै सकै छियै ।
