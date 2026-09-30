---
title: "Sınıf FastLZStream"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Aspose.Zip.FastLZ.FastLZStream sınıfı. FastLZ ile verileri sıkıştıran bir akış sarmalayıcısı. Dekoratör desenini uygular"
type: docs
weight: 500
url: /tr/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

FastLZ ile veri sıkıştıran bir akış sarmalayıcı. Dekoratör desenini uygular.

```csharp
public class FastLZStream : Stream
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | `FastLZStream` sınıfının sıkıştırma için hazırlanmış yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Mevcut akışın okuma desteği olup olmadığını gösteren bir değeri alır. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Mevcut akışın konum değiştirme desteği olup olmadığını gösteren bir değeri alır. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Mevcut akışın yazma desteği olup olmadığını gösteren bir değeri alır. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Akışın bayt cinsinden uzunluğunu alır. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Mevcut akış içindeki konumu alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Mevcut akışı kapatır ve mevcut akışla ilişkili tüm kaynakları (soketler ve dosya tutamaçları gibi) serbest bırakır. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Bu akış için tüm tamponları temizler ve tamponlanmış verilerin temel cihaza yazılmasını sağlar. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Akıştan bir dizi bayt okur ve okunan bayt sayısı kadar konumu ilerletir. Desteklenmiyor. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Mevcut akış içindeki konumu ayarlar. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Mevcut akışın uzunluğunu ayarlar. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Sıkıştırma akışına bir dizi bayt yazar ve yazılan bayt sayısı kadar bu akıştaki mevcut konumu ilerletir. |

### Ayrıca Bakınız

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


