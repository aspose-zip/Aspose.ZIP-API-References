---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipAESEncryptionSettings constructeur. Initialisiert eine neue Instanz vonSevenZipAESEncryptionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Initialisiert eine neue Instanz von[`SevenZipAESEncryptionSettings`](../) Klasse.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | String | Passwort für die Verschlüsselung oder Entschlüsselung. |

### Beispiele

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Siehe auch

* class [SevenZipAESEncryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* Montage [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Initialisiert eine neue Instanz von[`SevenZipAESEncryptionSettings`](../) Klasse mit externer Chiffre.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cipher | SevenZipCipher | Benutzerdefinierte AES-Implementierung. |

### Beispiele

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Siehe auch

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* Montage [Aspose.Zip](../../../)


