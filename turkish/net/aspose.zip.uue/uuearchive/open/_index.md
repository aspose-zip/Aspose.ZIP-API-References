---
title: "UueArchive.Open"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "UueArchive yöntemi. Arşivi çözümleme için açar ve arşiv içeriğiyle bir akış sağlar"
type: docs
weight: 60
url: /tr/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Arşivi kod çözme için açar ve arşiv içeriğiyle bir akış sağlar.

```csharp
public Stream Open()
```

### Dönüş Değeri

Arşivin içeriğini temsil eden akış.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

Bir dosyanın orijinal içeriğini elde etmek için akıştan okuyun. Örnekler bölümüne bakın.

## Örnekler

Kullanım:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 ve üzeri - Stream.CopyTo yöntemini kullanın:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 ve öncesi - baytları manuel olarak kopyalayın:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


