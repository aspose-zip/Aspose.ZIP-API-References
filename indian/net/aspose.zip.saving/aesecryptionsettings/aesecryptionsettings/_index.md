---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: AesEcryptionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैAesEcryptionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`AesEcryptionSettings`](../) वर्ग.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| password | String | एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड। |
| method | EncryptionMethod | एल्गोरिथम विकल्प सिफर के ब्लॉक आकार को दर्शाता है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| NotSupportedException | *method* में से एक नहीं हैAES128 ,AES192 , याAES256. |

### उदाहरण

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### यह सभी देखें

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../aesecryptionsettings/)
* सभा [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`AesEcryptionSettings`](../)कक्षा एक पासवर्ड के बिना.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| method | EncryptionMethod | एल्गोरिथम विकल्प सिफर के ब्लॉक आकार को दर्शाता है। |

### यह सभी देखें

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../aesecryptionsettings/)
* सभा [Aspose.Zip](../../../)


