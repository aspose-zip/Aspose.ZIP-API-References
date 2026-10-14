---
title: "ZstandardSaveOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZStandard आर्काइव के लिए सेटिंग्स।"
type: docs
weight: 159
url: /hi/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

ZStandard अभिलेख के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को सेट करता है। |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है।

```

``````

File source = new File(\"huge.bin\");
ZstandardSaveOptions settings = new ZstandardSaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     ZstandardSaveOptions settings = new ZstandardSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है। |

