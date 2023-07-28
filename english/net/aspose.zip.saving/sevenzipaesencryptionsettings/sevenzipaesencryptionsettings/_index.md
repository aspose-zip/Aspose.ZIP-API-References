---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipAESEncryptionSettings constructor. Initializes a new instance of the SevenZipAESEncryptionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Initializes a new instance of the [`SevenZipAESEncryptionSettings`](../) class.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password for encryption or decryption. |

## Examples

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### See Also

* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Initializes a new instance of the [`SevenZipAESEncryptionSettings`](../) class with external cipher.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cipher | SevenZipCipher | Custom AES implementation. |

## Examples

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### See Also

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)


