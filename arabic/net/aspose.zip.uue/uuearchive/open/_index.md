---
title: "UueArchive.Open"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة UueArchive. يفتح الأرشيف للفك ويُوفر تدفقًا بمحتوى الأرشيف"
type: docs
weight: 60
url: /ar/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

يفتح الأرشيف للفك ويُوفر دفقًا بمحتوى الأرشيف.

```csharp
public Stream Open()
```

### قيمة الإرجاع

التدفق الذي يمثل محتويات الأرشيف.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

## أمثلة

الاستخدام:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 وما فوق - استخدم طريقة Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 وما قبله - انسخ البايتات يدويًا:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### انظر أيضًا

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


