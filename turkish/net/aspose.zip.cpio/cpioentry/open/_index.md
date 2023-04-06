---
title: CpioEntry.Open
second_title: Aspose.ZIP for .NET API Referansı
description: CpioEntry yöntem. Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar.
type: docs
weight: 70
url: /tr/net/aspose.zip.cpio/cpioentry/open/
---
## CpioEntry.Open method

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

* class [CpioEntry](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioentry/)
* toplantı [Aspose.Zip](../../../)


