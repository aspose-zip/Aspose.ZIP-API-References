---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipAESEncryptionSettings constructeur. Initialiseert een nieuw exemplaar van hetSevenZipAESEncryptionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`SevenZipAESEncryptionSettings`](../) klasse.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | String | Wachtwoord voor codering of decodering. |

### Voorbeelden

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Zie ook

* class [SevenZipAESEncryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* montage [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Initialiseert een nieuw exemplaar van het[`SevenZipAESEncryptionSettings`](../) klasse met extern cijfer.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cipher | SevenZipCipher | Aangepaste AES-implementatie. |

### Voorbeelden

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Zie ook

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* montage [Aspose.Zip](../../../)


