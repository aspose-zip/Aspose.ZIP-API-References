---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "Apple Archive .aar फ़ाइल के भीतर LZMA संपीड़न के लिए सेटिंग्स।"
type: docs
weight: 23
url: /hi/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) फ़ाइल के भीतर LZMA संपीड़न के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | नए [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है। |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | नए [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है। |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | नए [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है। |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | डिफ़ॉल्ट पैरामीटरों के साथ [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | कम्प्रेशन से पहले प्रत्येक डेटा ब्लॉक का आकार प्राप्त करता है। |
| [getDictionarySize()](#getDictionarySize--) | कम्प्रेशन के लिए उपयोग किए जाने वाले शब्दकोश का आकार प्राप्त करता है। |
| [getFastBytes()](#getFastBytes--) | कम्प्रेशन के लिए उपयोग किए जाने वाले फास्ट बाइट्स की संख्या प्राप्त करता है। |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


नए [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| blockSize | int | कम्प्रेशन से पहले प्रत्येक डेटा ब्लॉक का आकार। |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


नए [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| blockSize | int | कम्प्रेशन से पहले प्रत्येक डेटा ब्लॉक का आकार। |
| dictionarySize | int | कम्प्रेशन के लिए उपयोग किया गया शब्दकोश आकार। |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


नए [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| blockSize | int | कम्प्रेशन से पहले प्रत्येक डेटा ब्लॉक का आकार। |
| dictionarySize | int | कम्प्रेशन के लिए उपयोग किया गया शब्दकोश आकार। |
| fastBytes | int | कम्प्रेशन के लिए उपयोग किए गए फास्ट बाइट्स की संख्या। |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


डिफ़ॉल्ट पैरामीटरों के साथ [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) क्लास का नया उदाहरण प्रारंभ करता है।

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


कम्प्रेशन से पहले प्रत्येक डेटा ब्लॉक का आकार प्राप्त करता है।

मान: डिफ़ॉल्ट मान 4 MiB है।

**Returns:**
int - कम्प्रेशन से पहले प्रत्येक डेटा ब्लॉक का आकार।
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


कम्प्रेशन के लिए उपयोग किए जाने वाले शब्दकोश का आकार प्राप्त करता है।

मान: डिफ़ॉल्ट मान 8 MiB है।

**Returns:**
int - कम्प्रेशन के लिए उपयोग किया गया शब्दकोश आकार।
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


कम्प्रेशन के लिए उपयोग किए जाने वाले फास्ट बाइट्स की संख्या प्राप्त करता है।

मान: डिफ़ॉल्ट मान 32 है।

**Returns:**
int - कम्प्रेशन के लिए उपयोग किए गए फास्ट बाइट्स की संख्या।
