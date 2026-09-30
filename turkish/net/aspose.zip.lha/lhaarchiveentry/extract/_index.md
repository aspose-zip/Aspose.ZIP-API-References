---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LhaArchiveEntry yöntemi. Lha arşiv girdisini bir dosya sistemine yol ile çıkarır"
type: docs
weight: 60
url: /tr/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Lha arşiv girdisini yola göre bir dosya sistemine çıkarır.

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
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| InvalidDataException | Veri geçersiz veya bozuk olduğunda fırlatılır. |

## Örnekler

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Ayrıca Bakınız

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
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
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| InvalidDataException | Veri geçersiz veya bozuk olduğunda fırlatılır. |

## Açıklamalar

Dizin girdisi için hiçbir şey yapmaz.

### Ayrıca Bakınız

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Lha arşiv girdisini bir dosyaya çıkarır.

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
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |

## Açıklamalar

Dizin girdisi için hiçbir şey yapmaz.

## Örnekler

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ayrıca Bakınız

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


