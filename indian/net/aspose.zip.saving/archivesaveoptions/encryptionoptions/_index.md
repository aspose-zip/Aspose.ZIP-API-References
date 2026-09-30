---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ArchiveSaveOptions प्रॉपर्टी। मौजूदा ZIP आर्काइव को सेव करने के लिए एन्क्रिप्शन सेटिंग्स को प्राप्त या सेट करता है"
type: docs
weight: 60
url: /hi/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

मौजूदा ZIP आर्काइव को सेव करने के लिए एन्क्रिप्शन सेटिंग्स को प्राप्त या सेट करता है।

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## टिप्पणियाँ

एनक्रिप्टेड आर्काइव की नियमित संरचना के लिए इन विकल्पों का उपयोग न करें, इसके बजाय [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) का उपयोग करें।

[`DataDescriptorPolicy`](../datadescriptorpolicy/) के साथ संगत नहीं है जिसका मान ForAllFileEntries है

## उदाहरण

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### संबंधित देखें

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


