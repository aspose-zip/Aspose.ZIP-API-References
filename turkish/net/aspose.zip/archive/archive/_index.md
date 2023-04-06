---
title: Archive.Archive
second_title: Aspose.ZIP for .NET API Referansı
description: Archive inşaatçı. Yeni bir örneğini başlatır.Archive girişleri için isteğe bağlı ayarlara sahip sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Yeni bir örneğini başlatır.[`Archive`](../) girişleri için isteğe bağlı ayarlara sahip sınıf.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Yeni eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) items. Belirtilmezse, şifreleme olmadan en yaygın Deflate sıkıştırması kullanılır. |

### Örnekler

Aşağıdaki örnek, tek bir dosyanın varsayılan ayarlarla nasıl sıkıştırılacağını gösterir.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Ayrıca bakınız

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Yeni bir örneğini başlatır.[`Archive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. |
| loadOptions | ArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |
| newEntrySettings | ArchiveEntrySettings | Yeni eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) items. Belirtilmezse, şifreleme olmadan en yaygın Deflate sıkıştırması kullanılır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *sourceStream* aranmaz. |
| InvalidDataException | AES için şifreleme başlığı, WinZip sıkıştırma yöntemiyle çelişiyor. |

### Notlar

Bu yapıcı herhangi bir girdiyi açmaz. Görmek[`Open`](../../archiveentry/open/) açma yöntemi.

### Örnekler

Aşağıdaki örnek, şifrelenmiş bir arşivi ayıklar, ardından ilk girdiyi sıkıştırılmış bir dosyaya açar.`Bellek Akışı`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ayrıca bakınız

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Yeni bir örneğini başlatır.[`Archive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının tam veya göreli yolu. |
| loadOptions | ArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |
| newEntrySettings | ArchiveEntrySettings | Yeni eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) items. Belirtilmezse, şifreleme olmadan en yaygın Deflate sıkıştırması kullanılır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Notlar

Bu yapıcı herhangi bir girdiyi açmaz. Görmek[`Open`](../../archiveentry/open/) açma yöntemi.

### Örnekler

Aşağıdaki örnek, şifrelenmiş bir arşivi ayıklar, ardından ilk girdiyi sıkıştırılmış bir dosyaya açar.`Bellek Akışı`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ayrıca bakınız

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)


