---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP for .NET API Referansı
description: SplitArchiveSaveOptions inşaatçı. Çok ciltli bir zip arşivini kaydetmek için ayarları başlatır.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Çok ciltli bir zip arşivini kaydetmek için ayarları başlatır.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Ciltlerin adı. .zip uzantılı veya uzantısız olabilir. |
| segmentSize | UInt32 | Hacim boyutu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | Segment boyutu 65536 bayttan küçük. |

### Notlar

Bazı hacimler şundan daha az olabilir:*segmentSize*. Çoğu durumda, son segment daha az olacaktır, ancak nadiren normal segmentler de olabilir.

Dosya adları aşağıdaki gibi olacaktır:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.zip.

### Ayrıca bakınız

* class [SplitArchiveSaveOptions](../)
* ad alanı [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* toplantı [Aspose.Zip](../../../)


