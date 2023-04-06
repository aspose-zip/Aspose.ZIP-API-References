---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: AesEcryptionSettings constructeur. Initialisiert eine neue Instanz vonAesEcryptionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Initialisiert eine neue Instanz von[`AesEcryptionSettings`](../) Klasse.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | String | Passwort für die Verschlüsselung oder Entschlüsselung. |
| method | EncryptionMethod | Algorithmusoption, die die Blockgröße der Chiffre angibt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| NotSupportedException | *method* ist keiner vonAES128 ,AES192 , oderAES256. |

### Beispiele

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Siehe auch

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../aesecryptionsettings/)
* Montage [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Initialisiert eine neue Instanz von[`AesEcryptionSettings`](../)Klasse ohne Passwort.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| method | EncryptionMethod | Algorithmusoption, die die Blockgröße der Chiffre angibt. |

### Siehe auch

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../aesecryptionsettings/)
* Montage [Aspose.Zip](../../../)


