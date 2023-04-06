---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Bzip2SaveOptions constructor. Inicializa una nueva instancia delBzip2SaveOptions clase.
type: docs
weight: 10
url: /es/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Inicializa una nueva instancia del[`Bzip2SaveOptions`](../) clase.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| blockSize | Int32 | Tamaño del bloque en cientos de kilobytes. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | El tamaño del bloque no está en el rango válido. |

### Ejemplos

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### Ver también

* class [Bzip2SaveOptions](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* asamblea [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Inicializa una nueva instancia del[`Bzip2SaveOptions`](../) clase con tamaño de bloque predeterminado, igual a 9 cientos de kilobytes.

```csharp
public Bzip2SaveOptions()
```

### Ejemplos

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### Ver también

* class [Bzip2SaveOptions](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* asamblea [Aspose.Zip](../../../)


