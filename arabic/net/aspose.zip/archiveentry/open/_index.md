---
title: ArchiveEntry.Open
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveEntry طريقة. يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى إدخال غير مضغوط.
type: docs
weight: 110
url: /ar/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى إدخال غير مضغوط.

```csharp
public Stream Open(string password = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| password | String | كلمة مرور اختيارية لفك التشفير. |

### قيمة الإرجاع

الدفق الذي يمثل محتويات الإدخال.

### ملاحظات

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. انظر قسم الأمثلة.

### أمثلة

الاستخدام:

.NET 4.0 والإصدارات الأحدث - استخدم طريقة Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 وما قبله - نسخ البايت يدويًا:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### أنظر أيضا

* class [ArchiveEntry](../)
* مساحة الاسم [Aspose.Zip](../../archiveentry/)
* المجسم [Aspose.Zip](../../../)


