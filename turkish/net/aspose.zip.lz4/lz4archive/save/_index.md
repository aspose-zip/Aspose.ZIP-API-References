---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Lz4Archive yöntemi. lz4 arşivini sağlanan akışa kaydeder"
type: docs
weight: 60
url: /tr/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Verilen akışa lz4 arşivini kaydeder.

```csharp
public void Save(Stream output)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çıktı | Akış | Hedef akış. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *output* null. |
| ArgumentException | *output* yazılabilir değil. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmış. - veya - Kaynak sağlanmadı. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Sağlanan iptal tokeni ile sıkıştırma iptal edildiğinde fırlatılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

*output* must be seekable.

## Örnekler

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Verilen hedef dosyaya lz4 arşivini kaydeder.

```csharp
public void Save(FileInfo destination)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | FileInfo | FileInfo, hedef akış olarak açılacak. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| SecurityException | Çağıranın *destination* açmak için gerekli izni yok. |
| ArgumentException | Dosya yolu boş veya yalnızca boşluk içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu yalnızca okunabilir veya bir dizin. |
| ArgumentNullException | *destination* null. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Verilen hedef dosyaya arşivi kaydeder.

```csharp
public void Save(string destinationFileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *destinationFileName* null. |
| SecurityException | Çağıranın erişim için gerekli izni yok |
| ArgumentException | *destinationFileName* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | Dosya *destinationFileName*'a erişim reddedildi. |
| PathTooLongException | Belirtilen *destinationFileName*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *destinationFileName* konumundaki dosya, dizenin ortasında bir iki nokta üst üste (:) içeriyor. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, (örneğin, eşlenmemiş bir sürücüde bulunması). |
| FileNotFoundException | *destinationFileName* içinde belirtilen dosya bulunamadı. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |

## Örnekler

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


