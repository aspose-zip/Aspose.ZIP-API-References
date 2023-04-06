---
title: SharArchive.SharArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SharArchive constructor. Inicializa una nueva instancia delSharArchive clase.
type: docs
weight: 10
url: /es/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Inicializa una nueva instancia del[`SharArchive`](../) clase.

```csharp
public SharArchive()
```

### Ejemplos

El siguiente ejemplo muestra cómo comprimir un archivo.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Ver también

* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Ver también

* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)


