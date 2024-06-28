---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP for .NET API Reference
description: AesEcryptionSettings constructor. Initializes a new instance of the AesEcryptionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Initializes a new instance of the [`AesEcryptionSettings`](../) class.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password for encryption or decryption. |
| method | EncryptionMethod | Algorithm option indicating block size of cipher. |

### Exceptions

| exception | condition |
| --- | --- |
| NotSupportedException | *method* is not one of AES128, AES192, or AES256. |

## Examples

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### See Also

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Initializes a new instance of the [`AesEcryptionSettings`](../) class without a password.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parameter | Type | Description |
| --- | --- | --- |
| method | EncryptionMethod | Algorithm option indicating block size of cipher. |

### See Also

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)


