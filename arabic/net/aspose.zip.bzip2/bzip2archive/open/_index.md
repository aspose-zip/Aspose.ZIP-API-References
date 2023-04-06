---
title: Bzip2Archive.Open
second_title: Aspose.ZIP لمرجع .NET API
description: Bzip2Archive طريقة. يفتح الأرشيف للاستخراج ويوفر دفقًا بمحتوى أرشيف.
type: docs
weight: 40
url: /ar/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

يفتح الأرشيف للاستخراج ويوفر دفقًا بمحتوى أرشيف.

```csharp
public Stream Open()
```

### قيمة الإرجاع

الدفق الذي يمثل محتويات الأرشيف.

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
Stream decompressed = archive.Open();
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)


