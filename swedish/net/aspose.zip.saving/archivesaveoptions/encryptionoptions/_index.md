---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ArchiveSaveOptions-egenskap. Hämtar eller anger krypteringsinställningar för att spara befintligt ZIP-arkiv"
type: docs
weight: 60
url: /sv/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Hämtar eller anger krypteringsinställningar för att spara befintligt ZIP-arkiv.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Anmärkningar

Använd inte dessa alternativ för vanlig sammansättning av krypterat arkiv, använd [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) istället.

Inte kompatibel med [`DataDescriptorPolicy`](../datadescriptorpolicy/) med värdet ForAllFileEntries

## Exempel

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Se även

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


