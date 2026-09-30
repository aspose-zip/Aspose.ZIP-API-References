---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "SevenZipLoadOptions-Eigenschaft. Liest oder setzt das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen"
type: docs
weight: 30
url: /de/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Liest oder setzt das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen.

```csharp
public string DecryptionPassword { get; set; }
```

## Beispiele

Sie können das Entschlüsselungspasswort einmal bei der Archivextraktion angeben.

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

### Siehe auch

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


