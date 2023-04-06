---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SplitArchiveSaveOptions constructeur. Instancie les paramètres denregistrement dune archive zip multivolumes.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Instancie les paramètres d'enregistrement d'une archive zip multi-volumes.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | Nom des volumes. Peut être avec ou sans extension .zip. |
| segmentSize | UInt32 | Taille du volume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | La taille du segment est inférieure à 65 536 octets. |

### Remarques

Certains volumes peuvent être inférieurs à*segmentSize*. Dans la plupart des cas, le dernier segment sera inférieur, mais rarement les segments réguliers le seront aussi.

Les noms des fichiers seront les suivants :*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.zipper.

### Voir également

* class [SplitArchiveSaveOptions](../)
* espace de noms [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* Assemblée [Aspose.Zip](../../../)


