---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SplitSevenZipArchiveSaveOptions constructeur. Instancie les paramètres denregistrement dune archive 7z multivolumes.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instancie les paramètres d'enregistrement d'une archive 7z multi-volumes.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | Nom des volumes. Peut être avec ou sans extension .7z. |
| segmentSize | UInt32 | Taille du volume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* est inférieur à 100. |

### Remarques

Certains volumes peuvent être inférieurs à*segmentSize*. Dans la plupart des cas, le dernier segment sera inférieur, mais rarement les segments réguliers le seront aussi.

Les noms des fichiers seront les suivants :*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Voir également

* class [SplitSevenZipArchiveSaveOptions](../)
* espace de noms [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* Assemblée [Aspose.Zip](../../../)


