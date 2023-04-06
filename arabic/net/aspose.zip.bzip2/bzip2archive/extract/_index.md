---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: Bzip2Archive طريقة. لاستخراج الأرشيف إلى الدفق المقدم.
type: docs
weight: 30
url: /ar/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

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
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)


