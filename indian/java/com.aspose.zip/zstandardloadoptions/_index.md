---
title: "ZstandardLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "कम्प्रेस्ड फ़ाइल से  लोड करने के विकल्प।"
type: docs
weight: 158
url: /hi/java/com.aspose.zip/zstandardloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardLoadOptions
```

विकल्प जिनके साथ [ZstandardArchive](../../com.aspose.zip/zstandardarchive) को संकुचित फ़ाइल से लोड किया जाता है। निष्कर्षण पर उठाए गए इवेंट को शामिल करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ZstandardLoadOptions()](#ZstandardLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को सेट करता है। |
### ZstandardLoadOptions() {#ZstandardLoadOptions--}
```
public ZstandardLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को प्राप्त करता है।

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Zstandard archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZstandardLoadOptions options = new ZstandardLoadOptions();
         options.setCancellationFlag(cf);
         try (ZstandardArchive a = new ZstandardArchive("big.zstd", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

रद्दीकरण अक्सर कुछ डेटा के निष्कर्षण न होने का परिणाम देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | एक रद्दीकरण फ़्लैग जो निष्कर्षण ऑपरेशन को रद्द करने के लिए उपयोग किया जाता है। |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को सेट करता है।

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

