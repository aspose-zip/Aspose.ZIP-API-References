---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "FastLZStream yöntemi. Akıştan bir bayt dizisi okur ve akış içindeki konumu okunan bayt sayısı kadar ilerletir. Desteklenmez"
type: docs
weight: 90
url: /tr/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Akıştan bir dizi bayt okur ve okunan bayt sayısı kadar konumu ilerletir. Desteklenmiyor.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tampon | Byte[] | Bir bayt dizisi. Bu yöntem döndüğünde, tampon belirtilen bayt dizisini içerir ve offset ile (offset + count - 1) arasındaki değerler, geçerli kaynaktan okunan baytlarla değiştirilir. |
| ofset | Int32 | Tampon içinde, geçerli akıştan okunan verilerin depolanmaya başlanacağı sıfır tabanlı bayt offseti. |
| count | Int32 | Geçerli akıştan okunacak azami bayt sayısı. |

### Dönüş Değeri

Tampona okunan toplam bayt sayısı. Bu, istenen bayt sayısından daha az olabilir; çünkü o kadar bayt mevcut değilse ya da akışın sonuna gelinmişse sıfır (0) olabilir.

### İstisnalar

| istisna | koşul |
| --- | --- |
| NotSupportedException | İşlem desteklenmiyor. |

### Ayrıca Bakınız

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


