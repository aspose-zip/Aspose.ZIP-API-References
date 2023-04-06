---
title: Class SevenZipCipher
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Crypto.SevenZipCipher sınıf. 7zip şifreleme için kullanılan AES şifresi için temel sınıf.
type: docs
weight: 190
url: /tr/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

7-zip şifreleme için kullanılan AES şifresi için temel sınıf.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Geçerli dönüşümün yeniden kullanılıp kullanılamayacağını gösteren bir değer alır. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Birden çok bloğun dönüştürülüp dönüştürülemeyeceğini gösteren bir değer alır. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Giriş bloğu boyutunu alır. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Çıkış bloğu boyutunu alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Giriş bayt dizisinin belirtilen bölgesini dönüştürür ve elde edilen dönüşümü çıkış bayt dizisinin belirtilen bölgesine kopyalar. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Belirtilen bayt dizisinin belirtilen bölgesini dönüştürür. |

### Ayrıca bakınız

* ad alanı [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* toplantı [Aspose.Zip](../../)


