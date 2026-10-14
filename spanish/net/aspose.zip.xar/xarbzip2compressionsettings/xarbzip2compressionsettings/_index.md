---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "XarBzip2CompressionSettings constructor. Inicializa una nueva instancia de la clase XarBzip2CompressionSettings"
type: docs
weight: 10
url: /es/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Inicializa una nueva instancia de la clase [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| blockSize | Int32 | Tamaño de bloque en cientos de kilobytes. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | El tamaño de bloque no está entre 1 y 9. |

## Ejemplos

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Ver también

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Inicializa una nueva instancia de la clase [`XarBzip2CompressionSettings`](../) con el tamaño de bloque predeterminado, igual a 9 cientos de kilobytes.

```csharp
public XarBzip2CompressionSettings()
```

### Ver también

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


