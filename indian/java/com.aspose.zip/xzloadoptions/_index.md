---
title: "XzLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "लोड करने के विकल्प।"
type: docs
weight: 152
url: /hi/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

लोड करने के विकल्प [XzArchive](../../com.aspose.zip/xzarchive).

.NET Framework 4.0 और उसके बाद के संस्करणों में, निष्कर्षण को रद्द करने के लिए उपयोग किया जा सकता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है।

एक निश्चित समय के बाद lzip आर्काइव निष्कर्षण रद्द करें।

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

