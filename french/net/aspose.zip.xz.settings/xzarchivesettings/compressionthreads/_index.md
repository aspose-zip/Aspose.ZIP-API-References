---
title: "XzArchiveSettings.CompressionThreads"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété XzArchiveSettings. Obtient ou définit le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée"
type: docs
weight: 70
url: /fr/net/aspose.zip.xz.settings/xzarchivesettings/compressionthreads/
---
## XzArchiveSettings.CompressionThreads property

Obtient ou définit le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée.

```csharp
public int CompressionThreads { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Le nombre de threads est supérieur à 100. |

## Remarques

Ne définissez pas ce nombre à plus que le nombre de cœurs CPU.

### Voir aussi

* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)


