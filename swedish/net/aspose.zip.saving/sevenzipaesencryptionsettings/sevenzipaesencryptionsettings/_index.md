---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipAESEncryptionSettings byggare. Initierar en ny instans avSevenZipAESEncryptionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Initierar en ny instans av[`SevenZipAESEncryptionSettings`](../) class.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| password | String | Lösenord för kryptering eller dekryptering. |

### Exempel

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Se även

* class [SevenZipAESEncryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Initierar en ny instans av[`SevenZipAESEncryptionSettings`](../) klass med extern chiffer.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cipher | SevenZipCipher | Anpassad AES-implementering. |

### Exempel

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Se även

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* hopsättning [Aspose.Zip](../../../)


