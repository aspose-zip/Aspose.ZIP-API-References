---
title: "XarFileEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل إدخال ملف داخل أرشيف xar."
type: docs
weight: 141
url: /ar/java/com.aspose.zip/xarfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class XarFileEntry extends XarEntry implements IArchiveFileEntry
```

تمثل إدخال ملف داخل أرشيف xar.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getCompressionProgressed()](#getCompressionProgressed--) | يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [open()](#open--) | يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

استخرج مدخلًا من أرشيف wim.

```

``````

try (FileOutputStream output = new FileOutputStream("file")){
try (XarArchive archive = new XarArchive("archive.xar")) {
((XarFileEntry)archive.getEntries().get(0)).extract(output);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         ((XarFileEntry)archive.getEntries().get(0)).extract("data.bin");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - معلومات الملف المستخرج
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

**Returns:**
java.io.InputStream - الدفق الذي يمثل محتويات العنصر
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

