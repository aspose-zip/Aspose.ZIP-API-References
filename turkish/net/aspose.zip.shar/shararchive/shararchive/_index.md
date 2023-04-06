---
title: SharArchive.SharArchive
second_title: Aspose.ZIP for .NET API Referansı
description: SharArchive inşaatçı. Yeni bir örneğini başlatır.SharArchive sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Yeni bir örneğini başlatır.[`SharArchive`](../) sınıf.

```csharp
public SharArchive()
```

### Örnekler

Aşağıdaki örnek, bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)


