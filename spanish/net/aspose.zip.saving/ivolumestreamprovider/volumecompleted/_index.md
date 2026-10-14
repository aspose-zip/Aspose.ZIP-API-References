---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método IVolumeStreamProvider. Se llama después de que se ha escrito un volumen de un archivo multivolumen dividido"
type: docs
weight: 20
url: /es/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Se llama después de que se haya escrito un volumen de un archivo dividido (multivolumen).

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El número de volúmenes escritos, comenzando desde cero. |
| s | Flujo | El flujo de destino al que se escribe el volumen. |
| isLast | Boolean | Indica si el volumen finaliza el archivo. |

### Ver también

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


