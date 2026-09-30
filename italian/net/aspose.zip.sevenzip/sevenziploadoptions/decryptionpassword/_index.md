---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà SevenZipLoadOptions. Ottiene o imposta la password per decrittare le voci e i nomi delle voci"
type: docs
weight: 30
url: /it/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Ottiene o imposta la password per decrittare le voci e i nomi delle voci.

```csharp
public string DecryptionPassword { get; set; }
```

## Esempi

È possibile fornire la password di decrittazione una sola volta durante l'estrazione dell'archivio.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


