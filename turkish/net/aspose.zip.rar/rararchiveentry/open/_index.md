---
title: RarArchiveEntry.Open
second_title: Aspose.ZIP for .NET API Referansı
description: RarArchiveEntry yöntem. Çıkarma için girişi açar ve sıkıştırılmış giriş içeriğiyle bir akış sağlar.
type: docs
weight: 100
url: /tr/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

Çıkarma için girişi açar ve sıkıştırılmış giriş içeriğiyle bir akış sağlar.

```csharp
public Stream Open(string password = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| password | String | Şifre çözme için isteğe bağlı şifre. içinde de ayarlanabilir[`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/). |

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

* class [RarArchiveEntry](../)
* ad alanı [Aspose.Zip.Rar](../../rararchiveentry/)
* toplantı [Aspose.Zip](../../../)


