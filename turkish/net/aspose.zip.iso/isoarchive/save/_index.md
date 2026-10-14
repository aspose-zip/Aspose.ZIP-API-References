---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoArchive yöntemi. ISO görüntüsünü belirtilen yola kaydeder"
type: docs
weight: 70
url: /tr/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

ISO görüntüsünü belirtilen yola kaydeder.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | ISO görüntüsünün kaydedileceği yol. |
| saveOptions | IsoSaveOptions | ISO arşivi kaydetmek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv düzenleme modunda olmadığında atılır. |
| ArgumentNullException | *path* null olduğunda atılır. |
| DirectoryNotFoundException | Belirtilen yol geçersiz olduğunda, örneğin eşlenmemiş bir sürücüde olduğunda atılır. |
| IOException | Dosya zaten açık olduğunda atılır. |
| UnauthorizedAccessException | Dosya *path* erişimi reddedildiğinde atılır. |
| PathTooLongException | Belirtilen *path* sistem tarafından tanımlanan maksimum uzunluğu aştığında atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

Aşağıdaki örnek, bir ISO arşivinin bir dosyaya nasıl kaydedileceğini gösterir:

```csharp
// Yeni bir boş ISO arşivi oluştur
using(IsoArchive isoArchive = new IsoArchive())
{
    // Dosyaları ISO arşivine ekle
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO arşivini bir dosyaya kaydet
    isoArchive.Save("new_archive.iso");
}
```

### Ayrıca Bakınız

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

ISO görüntüsünü belirtilen akışa kaydeder.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | ISO görüntüsünün kaydedileceği akış. |
| saveOptions | IsoSaveOptions | ISO arşivi kaydetmek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv düzenleme modunda olmadığında atılır. |
| ArgumentNullException | *stream* null olduğunda atılır. |
| ArgumentException | Akış *stream* yazılabilir olmadığında atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| IOException | Bir G/Ç hatası oluştu. |

## Örnekler

Aşağıdaki örnek, bir ISO arşivini bellek akışına nasıl kaydedeceğinizi gösterir:

```csharp

 // Yeni bir boş ISO arşivi oluştur
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Dosyaları ISO arşivine ekle
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // ISO arşivini bir bellek akışına kaydedin
     isoArchive.Save(memoryStream);
 }
```

### Ayrıca Bakınız

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


