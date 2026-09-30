---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarArchive yöntemi. Belirli bir girdinin giriş listesinde ilk oluşumunu kaldırır"
type: docs
weight: 50
url: /tr/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Belirli bir girdinin giriş listesinde ilk oluşumunu kaldırır.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| giriş | XarEntry | Giriş listesinden kaldırılacak girdi. |

### Dönüş Değeri

Xar entry örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *entry* null. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Arşiv çıkarma için açılmamış. |

## Örnekler

İşte son girdisi dışındaki tüm girdileri nasıl kaldırabileceğiniz:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Ayrıca Bakınız

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


