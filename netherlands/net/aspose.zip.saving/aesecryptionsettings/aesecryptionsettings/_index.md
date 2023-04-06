---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: AesEcryptionSettings constructeur. Initialiseert een nieuw exemplaar van hetAesEcryptionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`AesEcryptionSettings`](../) klasse.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | String | Wachtwoord voor codering of decodering. |
| method | EncryptionMethod | Algoritme-optie die de blokgrootte van het cijfer aangeeft. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| NotSupportedException | *method* is niet een vanAES128 ,AES192 , ofAES256. |

### Voorbeelden

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Zie ook

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../aesecryptionsettings/)
* montage [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Initialiseert een nieuw exemplaar van het[`AesEcryptionSettings`](../)klas zonder wachtwoord.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| method | EncryptionMethod | Algoritme-optie die de blokgrootte van het cijfer aangeeft. |

### Zie ook

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../aesecryptionsettings/)
* montage [Aspose.Zip](../../../)


