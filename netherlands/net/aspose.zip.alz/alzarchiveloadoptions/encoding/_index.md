---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AlzArchiveLoadOptions eigenschap. Haalt de codering voor itemnamen op of stelt deze in. Standaard is Koreaanse Windows‑codepagina 949 CP949"
type: docs
weight: 40
url: /nl/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Haalt de codering op of stelt deze in voor de namen van items. Standaard is Koreaanse Windows-codepagina 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Opmerkingen

ALZ-archieven slaan historisch gezien bestandsnamen op met behulp van de Koreaanse Windows ANSI‑codepagina.

## Voorbeelden

Itemnaam samengesteld met de opgegeven codering.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Zie ook

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


