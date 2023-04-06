---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP für .NET-API-Referenz
description: RarArchiveLoadOptions eigendom. Ruft das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen ab oder setzt es.
type: docs
weight: 20
url: /de/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Ruft das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen ab oder setzt es.

```csharp
public string DecryptionPassword { get; set; }
```

### Beispiele

Sie können das Entschlüsselungskennwort einmal beim Extrahieren des Archivs angeben.

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

### Siehe auch

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* namensraum [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* Montage [Aspose.Zip](../../../)


