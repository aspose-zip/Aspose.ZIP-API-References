---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Çok bölümlü 7-zip arşivi kaydetme seçenekleri."
type: docs
weight: 123
url: /tr/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Çok bölümlü 7-zip arşivi kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Çoklu hacimli 7z arşivi kaydetmek için ayarları oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFileName()](#getFileName--) | Uzantısız segmentlerin adını alır. |
| [getSegmentSize()](#getSegmentSize--) | Segmentin boyutunu alır. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Çoklu hacimli 7z arşivi kaydetmek için ayarları oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileName | java.lang.String | Hacimler için ad. .7z uzantısı ile ya da olmadan olabilir. |

Dosya adları aşağıdaki gibi olacaktır: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | hacmin boyutu. |

Bazı hacimler `segmentSize` değerinden daha küçük olabilir. Çoğu durumda, son segment daha küçük olur ancak nadiren normal segmentler de çok küçük olabilir. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Uzantısız segmentlerin adını alır.

**Returns:**
java.lang.String - uzantısız segmentlerin adı
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Segmentin boyutunu alır.

**Returns:**
long - segmentin boyutu.
