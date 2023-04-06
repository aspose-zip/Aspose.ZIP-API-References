---
title: Bzip2Archive.Open
second_title: Aspose.ZIP for .NET API Referansı
description: Bzip2Archive yöntem. Çıkarmak için arşivi açar ve arşiv içeriğine sahip bir akış sağlar.
type: docs
weight: 40
url: /tr/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Çıkarmak için arşivi açar ve arşiv içeriğine sahip bir akış sağlar.

```csharp
public Stream Open()
```

### Geri dönüş değeri

Arşivin içeriğini temsil eden akış.

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
Stream decompressed = archive.Open();
```

### Ayrıca bakınız

* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)


