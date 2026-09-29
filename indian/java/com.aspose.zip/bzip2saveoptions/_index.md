---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "bzip2 अभिलेख को सहेजने के विकल्प।"
type: docs
weight: 43
url: /hi/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

bzip2 अभिलेख को सहेजने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | नया उदाहरण प्रारंभ करता है [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) क्लास का। |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | डिफ़ॉल्ट ब्लॉक आकार के साथ नया उदाहरण प्रारंभ करता है [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) क्लास का, जो 9 सौ किलोबाइट के बराबर है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ब्लॉक आकार सौ किलोबाइट में। |
| [getCompressionProgressed()](#getCompressionProgressed--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [getCompressionThreads()](#getCompressionThreads--) | कम्प्रेशन थ्रेड की संख्या प्राप्त करता है। |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को सेट करता है। |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | कम्प्रेशन थ्रेड की संख्या सेट करता है। |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


नया उदाहरण प्रारंभ करता है [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) क्लास का।

```

``````

try (FileOutputStream result = new FileOutputStream(\"archive.bz2\")) {
try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save(result, new Bzip2SaveOptions(9));
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2SaveOptions() {#Bzip2SaveOptions--}
```
public Bzip2SaveOptions()
```


Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
         try (Bzip2Archive archive = new Bzip2Archive()) {
             archive.setSource("data.bin");
             archive.save(result, new Bzip2SaveOptions());
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


ब्लॉक आकार सौ किलोबाइट में।

**Returns:**
int - ब्लॉक आकार सौ किलोबाइट में
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है।

```

``````

File source = new File(\"huge.bin\");
Bzip2SaveOptions settings = new Bzip2SaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```

This event won't be raised when compressing in multithreaded mode.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     Bzip2SaveOptions settings = new Bzip2SaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```

यह इवेंट मल्टीथ्रेडेड मोड में कम्प्रेस करने पर नहीं उठाया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है। |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


कम्प्रेशन थ्रेड की संख्या सेट करता है। यदि मान 1 से बड़ा है, तो मल्टीथ्रेडिंग कम्प्रेशन उपयोग किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | कम्प्रेशन थ्रेड की संख्या। |

