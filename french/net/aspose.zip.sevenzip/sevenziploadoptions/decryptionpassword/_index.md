---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété SevenZipLoadOptions. Obtient ou définit le mot de passe pour déchiffrer les entrées et les noms d'entrées"
type: docs
weight: 30
url: /fr/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Obtient ou définit le mot de passe pour déchiffrer les entrées et les noms d'entrée.

```csharp
public string DecryptionPassword { get; set; }
```

## Exemples

Vous pouvez fournir le mot de passe de déchiffrement une fois lors de l'extraction de l'archive.

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

### Voir aussi

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


