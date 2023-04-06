---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TraditionalEncryptionSettings constructeur. Initialise une nouvelle instance duTraditionalEncryptionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Initialise une nouvelle instance du[`TraditionalEncryptionSettings`](../) classe.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| password | String | Mot de passe pour le cryptage. |

### Exemples

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Voir également

* class [TraditionalEncryptionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Initialise une nouvelle instance du[`TraditionalEncryptionSettings`](../) classe avec encodage défini par l'utilisateur.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| password | String | Mot de passe pour le cryptage. |
| encoding | Encoding | Encodage des caractères du mot de passe. |

### Remarques

L'utilisation de ce constructeur est déconseillée. La configuration de l'encodage peut contredire la norme et produire une archive incompatible.

### Exemples

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Voir également

* class [TraditionalEncryptionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Initialise une nouvelle instance du[`TraditionalEncryptionSettings`](../)classe sans mot de passe.

```csharp
public TraditionalEncryptionSettings()
```

### Voir également

* class [TraditionalEncryptionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* Assemblée [Aspose.Zip](../../../)


