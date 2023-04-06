---
title: ArchiveLoadOptions.Encoding
second_title: Referencia de la API de Aspose.ZIP para .NET
description: ArchiveLoadOptions propiedad. Obtiene o establece la codificación de los nombres de las entradas.
type: docs
weight: 30
url: /es/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Obtiene o establece la codificación de los nombres de las entradas.

```csharp
public Encoding Encoding { get; set; }
```

### Ejemplos

Nombre de entrada compuesto usando la codificación especificada independientemente de las propiedades del archivo zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Ver también

* class [ArchiveLoadOptions](../)
* espacio de nombres [Aspose.Zip](../../archiveloadoptions/)
* asamblea [Aspose.Zip](../../../)


