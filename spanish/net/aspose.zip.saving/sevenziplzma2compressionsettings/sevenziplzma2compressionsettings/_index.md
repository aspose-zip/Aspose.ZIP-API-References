---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipLZMA2CompressionSettings constructor. Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dictionarySize | Int32 | El tamaño del búfer de historial debe estar entre 4096 y 1073741824. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* es demasiado grande o demasiado pequeño. |

### Observaciones

Cuanto más grande es el diccionario, mejor suele ser la relación de compresión, pero los diccionarios más grandes que los datos sin comprimir son un desperdicio de RAM.

### Ver también

* class [SevenZipLZMA2CompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* asamblea [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dictionarySize | Int32 | El tamaño del búfer de historial debe estar entre 4096 y 1073741824. |
| fastBytes | Int32 | Controla el número de bytes rápidos utilizados por los compresores LZMA2. Una mayor cantidad de bytes rápidos puede proporcionar una mejor relación de compresión a expensas de la velocidad de compresión. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* es demasiado grande o demasiado pequeño, o*fastBytes* es demasiado grande o demasiado pequeño. |

### Observaciones

Cuanto más grande es el diccionario, mejor suele ser la relación de compresión, pero los diccionarios más grandes que los datos sin comprimir son un desperdicio de RAM.

### Ver también

* class [SevenZipLZMA2CompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* asamblea [Aspose.Zip](../../../)


