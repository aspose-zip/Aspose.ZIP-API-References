---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AlzArchiveLoadOptions-Eigenschaft. Gibt die Kodierung für Eintragsnamen zurück oder legt sie fest. Standard ist die koreanische Windows-Codepage 949 CP949."
type: docs
weight: 40
url: /de/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Liest oder setzt die Kodierung für Eintragsnamen. Standard ist die koreanische Windows-Codepage 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Hinweise

ALZ-Archive speichern Dateinamen historisch mit der koreanischen Windows-ANSI-Codepage.

## Beispiele

Eintragsname wird mit der angegebenen Kodierung zusammengesetzt.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Siehe auch

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


