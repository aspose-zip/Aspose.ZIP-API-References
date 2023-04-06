---
title: GzipArchive.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: GzipArchive طريقة. لاستخراج الأرشيف إلى الدفق المقدم.
type: docs
weight: 40
url: /ar/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

لاستخراج الأرشيف إلى الدفق المقدم.

```csharp
public void Extract(Stream destination)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destination | Stream | تيار الوجهة. يجب أن يكون قابلاً للكتابة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *destination* لا يدعم الكتابة. |

### أمثلة

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)


