---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AlzArchiveLoadOptions-egenskap. Hämtar eller anger kodningen för postnamn. Standard är Koreansk Windows-kodpage 949 CP949."
type: docs
weight: 40
url: /sv/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Hämtar eller anger kodningen för posternas namn. Standard är koreansk Windows-kodpage 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Anmärkningar

ALZ-arkiv har historiskt lagrat filnamn med den koreanska Windows ANSI-kodpagen.

## Exempel

Postnamn sammansatt med angiven kodning.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Se även

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


