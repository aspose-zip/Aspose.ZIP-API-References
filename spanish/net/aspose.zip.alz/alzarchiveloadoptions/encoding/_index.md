---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad AlzArchiveLoadOptions. Obtiene o establece la codificación para los nombres de las entradas. El valor predeterminado es la página de códigos coreana de Windows 949 CP949."
type: docs
weight: 40
url: /es/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Obtiene o establece la codificación para los nombres de las entradas. El valor predeterminado es la página de códigos coreana de Windows 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Observaciones

Los archivos ALZ históricamente almacenan los nombres de archivo usando la página de códigos ANSI de Windows coreano.

## Ejemplos

Nombre de entrada compuesto usando la codificación especificada.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Ver también

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


