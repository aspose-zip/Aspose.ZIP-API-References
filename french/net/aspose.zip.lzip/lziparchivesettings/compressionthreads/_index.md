---
title: "LzipArchiveSettings.CompressionThreads"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété LzipArchiveSettings. Obtient ou définit le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée"
type: docs
weight: 70
url: /fr/net/aspose.zip.lzip/lziparchivesettings/compressionthreads/
---
## LzipArchiveSettings.CompressionThreads property

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

* class [LzipArchiveSettings](../)
* namespace [Aspose.Zip.Lzip](../../lziparchivesettings/)
* assembly [Aspose.Zip](../../../)


