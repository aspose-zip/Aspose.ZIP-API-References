---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Lz4Archive yöntemi. Arşivi belirtilen yoldaki dosyaya çıkarır"
type: docs
weight: 30
url: /tr/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Arşivi yola göre dosyaya çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

### Dönüş Değeri

Çıkarılan dosyanın bilgisi.

### İstisnalar

| istisna | koşul |
| --- | --- |
| EndOfStreamException | Kaynak akış çok kısadır. |
| InvalidDataException | Kod çözme sırasında hatalı baytlar bulundu. |
| NotSupportedException | Bu LZ4 sürümü desteklenmiyor. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Arşiv birleştirme için hazırlanmıştır. |

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Arşivi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | Akış | Hedef akış. Yazılabilir olmalıdır. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *destination* yazmayı desteklemiyor. |
| EndOfStreamException | Kaynak akış çok kısadır. |
| InvalidDataException | Kod çözme sırasında hatalı baytlar bulundu. |
| NotSupportedException | Bu LZ4 sürümü desteklenmiyor. |
| InvalidOperationException | Arşiv birleştirme için hazırlanmıştır. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


