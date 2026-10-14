---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AlzEntry yöntemi. Girişi sağlanan yola göre dosya sistemine çıkarır"
type: docs
weight: 60
url: /tr/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Girişi sağlanan yola göre dosya sistemine çıkarır.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |
| parola | String | Şifreleme çözme için isteğe bağlı parola. |

### Dönüş Değeri

Bir birleştirilmiş dosyanın dosya bilgisi.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| InvalidDataException | Arşiv bozulmuş. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| FileNotFoundException | Dosya bulunamadı. |

## Örnekler

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Ayrıca Bakınız

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Girişi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | Akış | Hedef akış. Yazılabilir olmalıdır. |
| parola | String | Şifreleme çözme için isteğe bağlı parola. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *destination* yazmayı desteklemiyor. |
| InvalidOperationException | Arşiv çıkarma için açılmadı. - veya - Bu giriş bir dizindir. |
| InvalidDataException | Giriş içinde hatalı veri. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |

## Örnekler

Parola ile ALZ arşivinden bir giriş çıkar.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Ayrıca Bakınız

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


