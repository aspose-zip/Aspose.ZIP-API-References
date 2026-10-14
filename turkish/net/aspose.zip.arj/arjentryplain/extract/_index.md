---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ArjEntryPlain yöntemi. Sağlanan yola göre girişi dosya sistemine çıkarır"
type: docs
weight: 40
url: /tr/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Girişi sağlanan yola göre dosya sistemine çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

### Dönüş Değeri

Bir birleştirilmiş dosyanın dosya bilgisi.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null veya boş. |
| ObjectDisposedException | Arşiv serbest bırakıldıysa fırlatılır. |
| FileNotFoundException | Dosya bulunamadı. |
| InvalidDataException | Başlıklar veya veri için sağlama toplamı eşleşmiyor. - veya - Arşiv bozulmuş. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşar. |
| NotImplementedException | Giriş, yöntem 4 ile sıkıştırılmış. |

## Örnekler

rar arşivinden iki girişi çıkar.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Ayrıca Bakınız

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

ARJ arşiv girişini bir dosyaya çıkarır.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileInfo | FileInfo | Sıkıştırılmış veriyi depolamak için FileInfo. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv başlıkları ve hizmet bilgileri okunmadı. |
| SecurityException | Çağıranın *fileInfo* açmak için gerekli izni yok. |
| ArgumentException | Dosya yolu boş veya yalnızca boşluk içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu yalnızca okunabilir veya bir dizin. |
| ArgumentNullException | *fileInfo* null. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldıysa fırlatılır. |
| InvalidDataException | Başlıklar veya veri için sağlama toplamı eşleşmiyor. - veya - Arşiv bozulmuş. |
| NotImplementedException | Giriş, yöntem 4 ile sıkıştırılmış. |

## Örnekler

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ayrıca Bakınız

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| NotImplementedException | Giriş, yöntem 4 ile sıkıştırılmış. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldıysa fırlatılır. |

### Ayrıca Bakınız

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


