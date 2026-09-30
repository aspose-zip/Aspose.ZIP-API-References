---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété AlzArchiveLoadOptions. Obtient ou définit le mot de passe pour déchiffrer les entrées"
type: docs
weight: 30
url: /fr/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Obtient ou définit le mot de passe pour déchiffrer les entrées.

```csharp
public string DecryptionPassword { get; set; }
```

## Exemples

Vous pouvez fournir le mot de passe de déchiffrement une fois lors de l'extraction de l'archive.

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

### Voir aussi

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


