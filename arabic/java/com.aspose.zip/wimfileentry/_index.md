---
title: "WimFileEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف wim."
type: docs
weight: 133
url: /ar/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف wim.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [open()](#open--) | يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

استخرج مدخلًا من أرشيف wim.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract(httpResponseStream);
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

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - معلومات الملف المستخرج
### getLength() {#getLength--}
```
public final Long getLength()
```


يحصل على طول المدخل بالبايت.

**Returns:**
java.lang.Long - طول الإدخال بالبايت
### open() {#open--}
```
public final InputStream open()
```


يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل.

الاستخدام:

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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
