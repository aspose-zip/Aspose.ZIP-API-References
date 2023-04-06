---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP för .NET API-referens
description: AesEcryptionSettings byggare. Initierar en ny instans avAesEcryptionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Initierar en ny instans av[`AesEcryptionSettings`](../) class.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| password | String | Lösenord för kryptering eller dekryptering. |
| method | EncryptionMethod | Algoritmalternativ som indikerar blockstorlek på chiffer. |

### Undantag

| undantag | skick |
| --- | --- |
| NotSupportedException | *method* är inte en avAES128 ,AES192 , ellerAES256. |

### Exempel

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Se även

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../aesecryptionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Initierar en ny instans av[`AesEcryptionSettings`](../)klass utan lösenord.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| method | EncryptionMethod | Algoritmalternativ som indikerar blockstorlek på chiffer. |

### Se även

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../aesecryptionsettings/)
* hopsättning [Aspose.Zip](../../../)


