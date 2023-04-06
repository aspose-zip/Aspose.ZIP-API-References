---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Bzip2CompressionSettings constructor. Inicializa una nueva instancia delBzip2CompressionSettings clase.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Inicializa una nueva instancia del[`Bzip2CompressionSettings`](../) clase.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| blockSize | Int32 | Tamaño del bloque en cientos de kilobytes. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | El tamaño del bloque no está entre 1 y 9. |

### Ejemplos

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ver también

* class [Bzip2CompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* asamblea [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Inicializa una nueva instancia del[`Bzip2CompressionSettings`](../) clase con tamaño de bloque predeterminado, igual a 9 cientos de kilobytes.

```csharp
public Bzip2CompressionSettings()
```

### Ejemplos

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ver también

* class [Bzip2CompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* asamblea [Aspose.Zip](../../../)


