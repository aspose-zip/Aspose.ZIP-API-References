---
title: CpioEntry.Open
second_title: Aspose.ZIP لمرجع .NET API
description: CpioEntry طريقة. يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى الإدخال.
type: docs
weight: 70
url: /ar/net/aspose.zip.cpio/cpioentry/open/
---
## CpioEntry.Open method

يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى الإدخال.

```csharp
public Stream Open()
```

### قيمة الإرجاع

الدفق الذي يمثل محتويات الإدخال.

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

* class [CpioEntry](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioentry/)
* المجسم [Aspose.Zip](../../../)


