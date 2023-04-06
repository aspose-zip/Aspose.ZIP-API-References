---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Riferimento API Aspose.ZIP per .NET
description: RarArchiveLoadOptions proprietà. Ottiene o imposta la password per decrittografare le voci e i nomi delle voci.
type: docs
weight: 20
url: /it/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Ottiene o imposta la password per decrittografare le voci e i nomi delle voci.

```csharp
public string DecryptionPassword { get; set; }
```

### Esempi

È possibile fornire la password di decrittazione una volta all'estrazione dell'archivio.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.rar"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (RarArchive archive = new RarArchive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

### Guarda anche

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* spazio dei nomi [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* assemblea [Aspose.Zip](../../../)


