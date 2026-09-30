---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà AlzArchiveLoadOptions. Ottiene o imposta la password per decrittare le voci"
type: docs
weight: 30
url: /it/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Ottiene o imposta la password per decrittare le voci.

```csharp
public string DecryptionPassword { get; set; }
```

## Esempi

È possibile fornire la password di decrittazione una sola volta durante l'estrazione dell'archivio.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.alz"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
        {
            using (var decompressed = archive.Entries[0].Open())
            {
                byte[] b = new byte[8192];
                int bytesRead;
                while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
                    extracted.Write(b, 0, bytesRead);
                
            }
        }
    }
}
```

### Vedi anche

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


