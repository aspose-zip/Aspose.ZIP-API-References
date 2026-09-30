---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad ArchiveSaveOptions. Obtiene o establece la configuración de cifrado para guardar un archivo ZIP existente"
type: docs
weight: 60
url: /es/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Obtiene o establece la configuración de cifrado para guardar un archivo ZIP existente.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Observaciones

No utilice estas opciones para la composición regular de un archivo cifrado, use [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) en su lugar.

No compatible con [`DataDescriptorPolicy`](../datadescriptorpolicy/) con el valor ForAllFileEntries

## Ejemplos

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Ver también

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


