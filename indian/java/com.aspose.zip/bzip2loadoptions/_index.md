---
title: "Bzip2LoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "लोड करने के विकल्प।"
type: docs
weight: 42
url: /hi/java/com.aspose.zip/bzip2loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2LoadOptions
```

[Bzip2Archive](../../com.aspose.zip/bzip2archive) को लोड करने के विकल्प। निष्कर्षण पर उत्पन्न इवेंट शामिल है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Bzip2LoadOptions()](#Bzip2LoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को सेट करता है। |
### Bzip2LoadOptions() {#Bzip2LoadOptions--}
```
public Bzip2LoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को प्राप्त करता है।

```

``````

int[] percent = { 0 };
long originalFileLength = 10_000_000;

Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
});
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Bzip2 archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         Bzip2LoadOptions options = new Bzip2LoadOptions();
         options.setCancellationFlag(cf);
         try (Bzip2Archive a = new Bzip2Archive("big.bz2", options)) {
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

int[] percent = { 0 };
long originalFileLength = 10_000_000;

Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
});
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

