---
title: "ZArchiveSaveOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات Zarchive."
type: docs
weight: 155
url: /ar/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

إعدادات Zarchive.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام. |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام.

```

``````

File source = new File("huge.bin");
ZArchiveSaveOptions settings = new ZArchiveSaveOptions();
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
     ZArchiveSaveOptions settings = new ZArchiveSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | حدث يتم إطلاقه عندما يتم ضغط جزء من الدفق الخام. |

