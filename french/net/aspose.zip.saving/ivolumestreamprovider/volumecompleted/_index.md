---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode IVolumeStreamProvider. Appelée après qu'un volume d'une archive multi‑volume fractionnée a été écrit"
type: docs
weight: 20
url: /fr/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Appelé après qu'un volume d'une archive fractionnée (multivolume) a été écrit.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| index | Int32 | Le nombre de volumes écrits, à partir de zéro. |
| s | Stream | Le flux de destination vers lequel le volume est écrit. |
| isLast | Boolean | Indique si le volume termine l'archive. |

### Voir aussi

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


