---
title: "Bzip2SaveOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات حفظ أرشيف bzip2."
type: docs
weight: 43
url: /ar/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

خيارات حفظ أرشيف bzip2.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | ينشئ نسخة جديدة من الفئة [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions). |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | ينشئ نسخة جديدة من الفئة [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) بحجم كتلة افتراضي يساوي 9 مئات من الكيلوبايت. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | حجم الكتلة بالمئات من الكيلوبايت. |
| [getCompressionProgressed()](#getCompressionProgressed--) | يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [getCompressionThreads()](#getCompressionThreads--) | يحصل على عدد خيوط الضغط. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | يضبط عدد خيوط الضغط. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


ينشئ نسخة جديدة من الفئة [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions).

```

``````

try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(\"data.bin\");
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


حجم الكتلة بالمئات من الكيلوبايت.

**Returns:**
int - حجم الكتلة بالمئات من الكيلوبايت
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام.

```

``````

File source = new File("huge.bin");
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

لن يتم رفع هذا الحدث عند الضغط في وضع متعدد الخيوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | حدث يتم إطلاقه عندما يتم ضغط جزء من الدفق الخام. |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


يضبط عدد خيوط الضغط. إذا كانت القيمة أكبر من 1، سيتم استخدام الضغط متعدد الخيوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | int | عدد خيوط الضغط. |

