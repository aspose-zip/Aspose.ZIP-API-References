---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "एक स्ट्रीम रैपर जो डेटा को FastLZ के साथ संपीड़ित करता है।"
type: docs
weight: 68
url: /hi/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

FastLZ के साथ डेटा को संपीड़ित करने वाला एक स्ट्रीम रैपर। डेकोरेटर पैटर्न को लागू करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | संपीड़न के लिए तैयार FastLZStream क्लास की नई इंस्टेंस को प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | वर्तमान स्ट्रीम को बंद करता है और वर्तमान स्ट्रीम से जुड़े सभी संसाधनों (जैसे सॉकेट और फ़ाइल हैंडल) को मुक्त करता है। |
| [flush()](#flush--) | इस स्ट्रीम के सभी बफ़र को साफ़ करता है और किसी भी बफ़र किए गए डेटा को आधारभूत डिवाइस पर लिखवाता है। |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | संपीड़ित स्ट्रीम में बाइट्स की एक श्रृंखला लिखता है और लिखे गए बाइट्स की संख्या के अनुसार इस स्ट्रीम में वर्तमान स्थिति को आगे बढ़ाता है। |
| [write(int b)](#write-int-) | निर्दिष्ट बाइट को इस आउटपुट स्ट्रीम में लिखता है। |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


संपीड़न के लिए तैयार FastLZStream क्लास की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.OutputStream | संपीड़ित डेटा को सहेजने के लिए स्ट्रीम |
| compressionLevel | int | तेज़ संपीड़न के लिए 1 उपयोग करें, बेहतर संपीड़न अनुपात के लिए 2 उपयोग करें। |

### close() {#close--}
```
public void close()
```


वर्तमान स्ट्रीम को बंद करता है और वर्तमान स्ट्रीम से जुड़े सभी संसाधनों (जैसे सॉकेट और फ़ाइल हैंडल) को मुक्त करता है।

### flush() {#flush--}
```
public void flush()
```


इस स्ट्रीम के सभी बफ़र को साफ़ करता है और किसी भी बफ़र किए गए डेटा को आधारभूत डिवाइस पर लिखवाता है।

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


संपीड़ित स्ट्रीम में बाइट्स की एक श्रृंखला लिखता है और लिखे गए बाइट्स की संख्या के अनुसार इस स्ट्रीम में वर्तमान स्थिति को आगे बढ़ाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| buffer | byte[] | बाइट्स का एक एरे। यह मेथड बफ़र से वर्तमान स्ट्रीम में count बाइट्स कॉपी करता है। |
| offset | int | बफ़र में शून्य-आधारित बाइट ऑफ़सेट जहाँ से वर्तमान स्ट्रीम में बाइट्स कॉपी करना शुरू किया जाता है। |
| count | int | वर्तमान स्ट्रीम में लिखे जाने वाले बाइट्स की संख्या। |

### write(int b) {#write-int-}
```
public void write(int b)
```


निर्दिष्ट बाइट को इस आउटपुट स्ट्रीम में लिखता है। `write` का सामान्य अनुबंध यह है कि एक बाइट आउटपुट स्ट्रीम में लिखी जाती है। लिखी जाने वाली बाइट तर्क `b` के आठ लो-ऑर्डर बिट्स हैं। `b` के 24 हाई-ऑर्डर बिट्स को नजरअंदाज़ किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| b | int | `byte` का अर्थ |

