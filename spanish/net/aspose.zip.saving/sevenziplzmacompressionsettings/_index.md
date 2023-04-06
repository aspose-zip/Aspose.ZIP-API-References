---
title: Class SevenZipLZMACompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Saving.SevenZipLZMACompressionSettings clase. Configuraciones para el método de compresión LZMA dentro del archivo 7z.
type: docs
weight: 580
url: /es/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

Configuraciones para el método de compresión LZMA dentro del archivo 7z.

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos sin comprimir recientemente procesados se mantienen en la memoria. Si no se establece, se elegirá de acuerdo con el tamaño de la entrada. |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | Obtiene el método de compresión o descompresión. |

### Observaciones

El algoritmo de cadena Lempel-Ziv-Markov (LZMA) es un algoritmo que se utiliza para realizar una compresión de datos sin pérdidas. Este algoritmo utiliza un esquema de compresión de diccionario algo similar al algoritmo LZ77 y presenta una relación de compresión alta y un tamaño de diccionario de compresión variable.

Ver más: https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm

### Ver también

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* espacio de nombres [Aspose.Zip.Saving](../../aspose.zip.saving/)
* asamblea [Aspose.Zip](../../)


