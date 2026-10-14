---
title: "IArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الواجهة تمثل أرشيفًا."
type: docs
weight: 161
url: /ar/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

هذه الواجهة تمثل أرشيفًا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد.

إذا لم يكن الدليل موجودًا، فسيتم إنشاؤه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دليل الوجهة | java.lang.String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف.

الأرشيفات للاستخدام في الضغط فقط، مثل gzip و bzip2 و lzip و lzma و lz4 و xz و z، تتكون من سجل واحد - الأرشيف نفسه.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - مدخلات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) تشكل الأرشيف.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
