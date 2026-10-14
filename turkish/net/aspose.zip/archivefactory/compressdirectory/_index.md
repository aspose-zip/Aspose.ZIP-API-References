---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ArchiveFactory yöntemi. Belirtilen dizini, sağlanan arşiv formatını kullanarak bir arşiv dosyasına sıkıştırır"
type: docs
weight: 10
url: /tr/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Belirtilen dizini, sağlanan arşiv formatını kullanarak bir arşiv dosyasına sıkıştırır.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Sıkıştırılacak dizinin yolu. |
| outputFileName | String | Hedef dosya adı. |
| archiveFormat | ArchiveFormat | Oluşturulacak arşivin formatı (ör. zip, rar, tar vb.). |

### İstisnalar

| istisna | koşul |
| --- | --- |
| DirectoryNotFoundException | *path* tarafından belirtilen dizin mevcut değilse fırlatılır. |
| ArgumentException | *path* null veya boş bir dize ise fırlatılır. |
| NotSupportedException | Belirtilen *archiveFormat* desteklenmiyor veya tanınmıyorsa fırlatılır. |
| ArgumentNullException | *path* `null`. |

## Açıklamalar

Bu yöntem, *path* parametresiyle belirtilen konumda bir arşiv dosyası oluşturur. Arşiv dosyasının adı genellikle dizin adı ve *archiveFormat*'a göre uygun dosya uzantısının birleştirilmesiyle oluşur. Dizin kendisi değiştirilmez veya silinmez.

## Örnekler

CompressDirectory yönteminin nasıl kullanılacağını gösteren bir örnek:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Bu, belirtilen yoldaki dizinin içeriğiyle bir ZIP dosyası oluşturur.
```

### Ayrıca Bakınız

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


