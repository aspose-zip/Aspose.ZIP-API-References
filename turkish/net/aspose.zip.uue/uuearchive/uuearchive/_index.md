---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "UueArchive yapıcı. Kodlamaya hazırlanmış bir UueArchive sınıfının yeni örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Kodlamaya hazırlanmış bir [`UueArchive`](../) sınıfının yeni örneğini başlatır.

```csharp
public UueArchive()
```

## Örnekler

Aşağıdaki örnek, bir dosyanın nasıl uuencode edileceğini gösterir.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Kod çözmeye hazırlanmış bir [`UueArchive`](../) sınıfının yeni örneğini başlatır.

```csharp
public UueArchive(Stream sourceStream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | Akış | Arşivin kaynağı. |

## Açıklamalar

Bu yapıcı kod çözmez. Çözmek için [`Open`](../open/) yöntemine bakın.

## Örnekler

Bir akıştan arşivi açın ve bir `MemoryStream`'e çıkarın

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Bir [`UueArchive`](../) sınıfının yeni örneğini başlatır.

```csharp
public UueArchive(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının yolu. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| FileNotFoundException | Dosya bulunamadı. |
| IOException | Dosya zaten açık. |

## Açıklamalar

Bu yapıcı sıkıştırmayı açmaz. Açmak için [`Open`](../open/) yöntemine bakın.

## Örnekler

Yolu belirtilen dosyadan bir arşivi aç ve onu bir `MemoryStream`'e çöz.

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


