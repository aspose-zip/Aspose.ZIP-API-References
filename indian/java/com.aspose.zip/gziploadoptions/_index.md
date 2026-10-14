---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "लोड करने के विकल्प।"
type: docs
weight: 70
url: /hi/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

लोड करने के विकल्प [GzipArchive](../../com.aspose.zip/gziparchive)।

.NET Framework 4.0 और उसके बाद के संस्करणों में, निष्कर्षण को रद्द करने के लिए उपयोग किया जा सकता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | स्ट्रीम हेडर को पार्स करके गुणों, जिसमें नाम भी शामिल है, निर्धारित करने के लिए मान प्राप्त करता है। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | स्ट्रीम हेडर को पार्स करके गुणों, जिसमें नाम भी शामिल है, निर्धारित करने के लिए मान सेट करता है। |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


स्ट्रीम हेडर को पार्स करके गुणों, जिसमें नाम भी शामिल है, निर्धारित करने के लिए मान प्राप्त करता है। यह केवल खोज योग्य स्ट्रीम के लिए ही अर्थपूर्ण है।

**Returns:**
बूलियन - स्ट्रीम हेडर को पार्स करके गुणों, जिसमें नाम भी शामिल है, निर्धारित करने के लिए मान।
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है।

एक निश्चित समय के बाद gzip आर्काइव निष्कर्षण को रद्द करें।

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("निकालना 60 सेकंड के बाद रद्द कर दिया गया");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

