---
title: WimFileEntry.Open
second_title: Aspose.ZIP for .NET API Referansı
description: WimFileEntry yöntem. Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar.
type: docs
weight: 30
url: /tr/net/aspose.zip.wim/wimfileentry/open/
---
## WimFileEntry.Open method

Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar.

```csharp
public Stream Open()
```

### Geri dönüş değeri

Girişin içeriğini temsil eden akış.

### Notlar

Dosyanın orijinal içeriğini almak için akıştan okuyun. Örnekler bölümüne bakın.

### Örnekler

Kullanım:

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

```csharp
Stream decompressed = entry.Open();
```

### Ayrıca bakınız

* class [WimFileEntry](../)
* ad alanı [Aspose.Zip.Wim](../../wimfileentry/)
* toplantı [Aspose.Zip](../../../)


