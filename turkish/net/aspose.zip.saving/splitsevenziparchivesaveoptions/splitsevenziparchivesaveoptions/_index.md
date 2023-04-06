---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP for .NET API Referansı
description: SplitSevenZipArchiveSaveOptions inşaatçı. Çok ciltli bir 7z arşivini kaydetmek için ayarları başlatır.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Çok ciltli bir 7z arşivini kaydetmek için ayarları başlatır.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Ciltlerin adı. .7z uzantılı veya uzantısız olabilir. |
| segmentSize | UInt32 | Hacim boyutu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* 100'den azdır. |

### Notlar

Bazı hacimler şundan daha az olabilir:*segmentSize*. Çoğu durumda, son segment daha az olacaktır, ancak nadiren normal segmentler de olabilir.

Dosya adları aşağıdaki gibi olacaktır:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Ayrıca bakınız

* class [SplitSevenZipArchiveSaveOptions](../)
* ad alanı [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* toplantı [Aspose.Zip](../../../)


