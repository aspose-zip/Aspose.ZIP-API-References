---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TraditionalEncryptionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैTraditionalEncryptionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`TraditionalEncryptionSettings`](../) वर्ग.

```csharp
public TraditionalEncryptionSettings(string password)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| password | String | एन्क्रिप्शन के लिए पासवर्ड। |

### उदाहरण

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [TraditionalEncryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* सभा [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`TraditionalEncryptionSettings`](../) उपयोगकर्ता परिभाषित एन्कोडिंग के साथ वर्ग।

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| password | String | एन्क्रिप्शन के लिए पासवर्ड। |
| encoding | Encoding | पासवर्ड वर्णों के लिए एन्कोडिंग। |

### टिप्पणियों

इस कन्स्ट्रक्टर का उपयोग निराश है। एन्कोडिंग सेट करना मानक के विपरीत हो सकता है और असंगत संग्रह उत्पन्न कर सकता है।

### उदाहरण

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [TraditionalEncryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* सभा [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`TraditionalEncryptionSettings`](../)कक्षा एक पासवर्ड के बिना.

```csharp
public TraditionalEncryptionSettings()
```

### यह सभी देखें

* class [TraditionalEncryptionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* सभा [Aspose.Zip](../../../)


