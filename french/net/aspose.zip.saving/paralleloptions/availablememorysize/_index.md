---
title: ParallelOptions.AvailableMemorySize
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ParallelOptions propriété. Obtient ou définit lestimation de la mémoire en mégaoctets disponibles pour accueillir les entrées compressées sans permuter sur le disque. Cette valeur na de sens que siParallelCompressInMemory le réglage est enAuto mode.
type: docs
weight: 20
url: /fr/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Obtient ou définit l'estimation de la mémoire en mégaoctets disponibles pour accueillir les entrées compressées sans permuter sur le disque. Cette valeur n'a de sens que si[`ParallelCompressInMemory`](../parallelcompressinmemory/) le réglage est enAuto mode.

```csharp
public int AvailableMemorySize { get; set; }
```

### Remarques

Cette valeur est utilisée pour calculer la plus grande taille d'entrée pouvant être compressée en parallèle avec d'autres. Toutes les entrées au-dessus du seuil calculé seront compressées séquentiellement. Il est sûr d'avoir`AvailableMemorySize` propriété aussi grande que la RAM libre et même plus grande. Par défaut, il est supposé que vous disposez d'au moins 200 Mo par cœur de processeur.

### Voir également

* class [ParallelOptions](../)
* espace de noms [Aspose.Zip.Saving](../../paralleloptions/)
* Assemblée [Aspose.Zip](../../../)


