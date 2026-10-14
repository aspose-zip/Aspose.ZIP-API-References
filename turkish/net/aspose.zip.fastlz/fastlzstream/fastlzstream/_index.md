---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "FastLZStream yapıcı. Sıkıştırma için hazırlanmış FastLZStream sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Sıkıştırma için hazırlanmış [`FastLZStream`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Sıkıştırılmış veriyi kaydetmek için akış. |
| compressionLevel | Int32 | Daha hızlı sıkıştırma için 1, daha iyi sıkıştırma oranı için 2 kullanın. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *stream* null. |
| ArgumentException | *stream* yazmayı desteklemiyor. |
| ArgumentOutOfRangeException | *compressionLevel* 2'den büyük ya da 1'den küçüktür. |

### Ayrıca Bakınız

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


