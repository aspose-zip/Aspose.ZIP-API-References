---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipAESEncryptionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैSevenZipAESEncryptionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`SevenZipAESEncryptionSettings`](../) वर्ग.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| password | String | एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड। |

### उदाहरण

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### यह सभी देखें

* class [SevenZipAESEncryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* सभा [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`SevenZipAESEncryptionSettings`](../) बाहरी सिफर के साथ वर्ग.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cipher | SevenZipCipher | कस्टम एईएस कार्यान्वयन। |

### उदाहरण

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### यह सभी देखें

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* सभा [Aspose.Zip](../../../)


