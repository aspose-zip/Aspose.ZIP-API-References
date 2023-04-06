---
title: SevenZipArchiveEntry.Open
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchiveEntry طريقة. يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى الإدخال.
type: docs
weight: 90
url: /ar/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى الإدخال.

```csharp
public Stream Open(string password = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| password | String | كلمة مرور اختيارية لفك التشفير. |

### قيمة الإرجاع

الدفق الذي يمثل محتويات الإدخال.

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | الأرشيف غير مفتوح للاستخراج. - أو - هذا الإدخال هو دليل. |
| InvalidDataException | بيانات خاطئة داخل الإدخال. |

### ملاحظات

اقرأ من البث للحصول على المحتوى الأصلي للملف. انظر قسم الأمثلة.

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

* class [SevenZipArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* المجسم [Aspose.Zip](../../../)


