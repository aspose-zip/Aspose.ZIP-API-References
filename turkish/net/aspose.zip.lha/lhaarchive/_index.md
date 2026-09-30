---
title: "Sınıf LhaArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Aspose.Zip.Lha.LhaArchive sınıfı. Bu sınıf bir LHA .lzh arşiv dosyasını temsil eder"
type: docs
weight: 630
url: /tr/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Bu sınıf bir LHA (.lzh) arşiv dosyasını temsil eder.

```csharp
public class LhaArchive : IArchive
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Yeni bir `LhaArchive` sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Yeni bir `LhaArchive` sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Arşivi oluşturan [`LhaArchiveEntry`](../lhaarchiveentry/) tipindeki dosya girdilerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Arşivdeki tüm dosya ve dizinleri verilen dizine çıkarır. |

## Açıklamalar

Yalnızca aşağıdaki sıkıştırma yöntemleri desteklenir:

**Method**

**Explanation**

**lh0**

Sıkıştırılmamış

**lh4**

8 KiB kaydırmalı sözlük ve statik Huffman

**lh5**

16 KiB kaydırmalı sözlük ve statik Huffman

**lh6**

64 KiB kaydırmalı sözlük ve statik Huffman

**lh7**

128 KiB kaydırmalı sözlük ve statik Huffman

**lhx**

1 Mib kaydırmalı sözlük ve statik Huffman

**lhd**

Dizin

### Ayrıca Bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


