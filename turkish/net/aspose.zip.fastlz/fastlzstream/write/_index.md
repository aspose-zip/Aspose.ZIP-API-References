---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "FastLZStream yöntemi. Sıkıştırma akışına bir bayt dizisi yazar ve bu akıştaki geçerli konumu yazılan bayt sayısı kadar ilerletir"
type: docs
weight: 120
url: /tr/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Sıkıştırma akışına bir dizi bayt yazar ve yazılan bayt sayısı kadar bu akıştaki mevcut konumu ilerletir.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tampon | Byte[] | Bir bayt dizisi. Bu yöntem, tampondan geçerli akışa count bayt kopyalar. |
| ofset | Int32 | Tampon içinde, baytların geçerli akışa kopyalanmaya başlanacağı sıfır tabanlı bayt offseti. |
| count | Int32 | Geçerli akışa yazılacak bayt sayısı. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Akış serbest bırakıldıysa fırlatılır. |
| ArgumentNullException | *buffer* `null`'dır. |

### Ayrıca Bakınız

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


