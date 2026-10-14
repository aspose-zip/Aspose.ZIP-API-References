---
title: "LzxLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "कम्प्रेस्ड फ़ाइल से अभिलेख लोड करने के विकल्प।"
type: docs
weight: 91
url: /hi/java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

कम्प्रेस्ड फ़ाइल से अभिलेख लोड करने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है।

एक निश्चित समय के बाद ISO आर्काइव निष्कर्षण रद्द करें।

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzxLoadOptions options = new LzxLoadOptions();
options.setCancellationFlag(cf);
try (LzxArchive a = new LzxArchive("big.lzx", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

