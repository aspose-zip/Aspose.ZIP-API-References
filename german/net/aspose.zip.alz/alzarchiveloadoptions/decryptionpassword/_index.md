---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AlzArchiveLoadOptions-Eigenschaft. Gibt das Passwort zum Entschlüsseln von Einträgen zurück oder legt es fest."
type: docs
weight: 30
url: /de/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Liest oder setzt das Passwort zum Entschlüsseln von Einträgen.

```csharp
public string DecryptionPassword { get; set; }
```

## Beispiele

Sie können das Entschlüsselungspasswort einmal bei der Archivextraktion angeben.

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

### Siehe auch

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


