---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveLoadOptions propriété. Obtient ou définit le mot de passe pour déchiffrer les entrées.
type: docs
weight: 20
url: /fr/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Obtient ou définit le mot de passe pour déchiffrer les entrées.

```csharp
public string DecryptionPassword { get; set; }
```

### Exemples

Vous pouvez fournir un mot de passe de déchiffrement une fois lors de l'extraction de l'archive.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.zip"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

### Voir également

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* espace de noms [Aspose.Zip](../../archiveloadoptions/)
* Assemblée [Aspose.Zip](../../../)


