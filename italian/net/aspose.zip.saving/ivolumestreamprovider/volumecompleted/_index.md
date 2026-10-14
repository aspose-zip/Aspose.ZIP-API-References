---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo IVolumeStreamProvider. Chiamato dopo che un volume di un archivio multivolume diviso è stato scritto"
type: docs
weight: 20
url: /it/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Chiamato dopo che un volume di un archivio diviso (multivolume) è stato scritto.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | Il numero di volumi scritti, a partire da zero. |
| s | Stream | Lo stream di destinazione a cui è stato scritto il volume. |
| isLast | Boolean | Indica se il volume termina l'archivio. |

### Vedi anche

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


