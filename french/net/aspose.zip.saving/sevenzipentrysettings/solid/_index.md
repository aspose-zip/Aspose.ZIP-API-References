---
title: "SevenZipEntrySettings.Solid"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété SevenZipEntrySettings. Obtient ou définit une valeur indiquant s'il faut concaténer les entrées et les traiter comme un seul bloc de données"
type: docs
weight: 50
url: /fr/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Obtient ou définit la valeur indiquant s'il faut concaténer les entrées et les traiter comme un seul bloc de données.

```csharp
public bool Solid { get; set; }
```

## Remarques

Fournit `SevenZipEntrySettings` pour une archive 7z solide lors de l'instanciation de l'archive.

## Exemples

L'exemple suivant montre comment compresser un répertoire en archive 7z solide avec compression LZMA2 sans chiffrement.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### Voir aussi

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


