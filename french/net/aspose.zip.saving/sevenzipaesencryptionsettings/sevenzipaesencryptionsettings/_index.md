---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipAESEncryptionSettings constructeur. Initialise une nouvelle instance duSevenZipAESEncryptionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Initialise une nouvelle instance du[`SevenZipAESEncryptionSettings`](../) classe.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| password | String | Mot de passe pour le chiffrement ou le déchiffrement. |

### Exemples

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Voir également

* class [SevenZipAESEncryptionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Initialise une nouvelle instance du[`SevenZipAESEncryptionSettings`](../) classe avec chiffrement externe.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| cipher | SevenZipCipher | Implémentation AES personnalisée. |

### Exemples

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Voir également

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* Assemblée [Aspose.Zip](../../../)


