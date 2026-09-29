---
title: "Lz4LoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "लोड करने के विकल्प।"
type: docs
weight: 82
url: /hi/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

[Lz4Archive](../../com.aspose.zip/lz4archive) लोड करने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है।

एक निश्चित समय के बाद lz4 संग्रह निष्कर्षण रद्द करें।

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
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

