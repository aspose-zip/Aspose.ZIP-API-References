---
title: Bzip2Archive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: Bzip2Archive yöntem. Arşivi sağlanan akışa kaydeder.
type: docs
weight: 50
url: /tr/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| outputStream | Stream | Hedef akışı. |
| saveOptions | Bzip2SaveOptions | Bir bzip2 arşivini kaydetme seçenekleri. Belirtilmemiş ise 900 Kb blok boyutu kullanılacaktır. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Arşivlenecek verilerin kaynağı sağlanmadı. |
| ArgumentException | *outputStream* yazılabilir değil. |
| UnauthorizedAccessException | Dosya kaynağı salt okunurdur veya bir dizindir. |
| DirectoryNotFoundException | Eşlenmemiş bir sürücüde olmak gibi, belirtilen dosya kaynağı yolu geçersiz. |
| IOException | Dosya kaynağı zaten açık. |

### Notlar

*outputStream*yazılabilir olmalıdır.

### Örnekler

Sıkıştırılmış verileri http yanıt akışına yazar.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Ayrıca bakınız

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Arşivi sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| saveOptions | Bzip2SaveOptions | Bir bzip2 arşivini kaydetme seçenekleri. Belirtilmemiş ise 900 Kb blok boyutu kullanılacaktır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *destinationFileName* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*destinationFileName* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*destinationFileName* engellendi. |
| PathTooLongException | Belirtilen*destinationFileName*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*destinationFileName* dizenin ortasında iki nokta üst üste (:) içerir. |

### Örnekler

Sıkıştırılmış verileri dosyaya yazar.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Ayrıca bakınız

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)


