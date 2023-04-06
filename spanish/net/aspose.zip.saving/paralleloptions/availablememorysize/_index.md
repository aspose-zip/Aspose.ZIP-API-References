---
title: ParallelOptions.AvailableMemorySize
second_title: Referencia de la API de Aspose.ZIP para .NET
description: ParallelOptions propiedad. Obtiene o establece la estimación de memoria en megabytes disponibles para acomodar las entradas comprimidas sin cambiar al disco. Este valor solo tiene sentido siParallelCompressInMemory el ajuste está enAuto modo.
type: docs
weight: 20
url: /es/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Obtiene o establece la estimación de memoria en megabytes disponibles para acomodar las entradas comprimidas sin cambiar al disco. Este valor solo tiene sentido si[`ParallelCompressInMemory`](../parallelcompressinmemory/) el ajuste está enAuto modo.

```csharp
public int AvailableMemorySize { get; set; }
```

### Observaciones

Este valor se utiliza para calcular el mayor tamaño de entrada que se puede comprimir en paralelo con otras. Todas las entradas por encima del umbral calculado se comprimirán secuencialmente. Es seguro tener`AvailableMemorySize` propiedad tan grande como RAM libre e incluso más grande. De forma predeterminada, se supone que tiene al menos 200 MB por núcleo de CPU.

### Ver también

* class [ParallelOptions](../)
* espacio de nombres [Aspose.Zip.Saving](../../paralleloptions/)
* asamblea [Aspose.Zip](../../../)


