---
title: "FastLZStream.FastLZStream"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor FastLZStream. Inicializa una nueva instancia de la clase FastLZStream preparada para compresión"
type: docs
weight: 10
url: /es/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Inicializa una nueva instancia de la clase [`FastLZStream`](../) preparada para compresión.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo para guardar datos comprimidos. |
| compressionLevel | Int32 | Use 1 para una compresión más rápida, use 2 para una mejor relación de compresión. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *stream* es nulo. |
| ArgumentException | *stream* no admite escritura. |
| ArgumentOutOfRangeException | *compressionLevel* es mayor que 2 o menor que 1. |

### Ver también

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


