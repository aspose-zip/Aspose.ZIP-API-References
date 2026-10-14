---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LzxArchiveEntry yöntemi. Lzx arşiv girdisini bir dosya sistemine yol ile çıkarır"
type: docs
weight: 80
url: /tr/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Lzx arşiv girişini yol ile bir dosya sistemine çıkarır.

```csharp
public FileSystemInfo Extract(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Açılmış verileri depolayacak dosyanın yolu. |

### Dönüş Değeri

Çıkarılan verileri içeren FileSystemInfoInstance.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv başlıkları ve hizmet bilgileri okunmadı. |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| InvalidDataException | Başlıklar veya veri için sağlama toplamı eşleşmiyor. - veya - Arşiv bozulmuş. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| NotSupportedException | Geçersiz sıkıştırma yöntemi. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| EndOfStreamException | Akışın sonuna beklenmedik bir şekilde ulaşıldığında fırlatılır. |

## Örnekler

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Ayrıca Bakınız

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Girişi sağlanan akışa çıkarır.

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
| InvalidDataException | Başlıklar veya veri için sağlama toplamı eşleşmiyor. - veya - Arşiv bozulmuş. |
| ArgumentNullException | Hedef akış null. |
| NotSupportedException | Geçersiz sıkıştırma yöntemi. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| EndOfStreamException | Akışın sonuna beklenmedik bir şekilde ulaşıldığında fırlatılır. |

### Ayrıca Bakınız

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


