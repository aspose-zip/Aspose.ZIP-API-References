---
title: SevenZipArchiveEntry.Open
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchiveEntry yöntem. Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar.
type: docs
weight: 90
url: /tr/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar.

```csharp
public Stream Open(string password = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| password | String | Şifre çözme için isteğe bağlı şifre. |

### Geri dönüş değeri

Girişin içeriğini temsil eden akış.

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Arşiv çıkartma için açılmadı. - veya - Bu girdi bir dizindir. |
| InvalidDataException | Girişte yanlış veri. |

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

* class [SevenZipArchiveEntry](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* toplantı [Aspose.Zip](../../../)


