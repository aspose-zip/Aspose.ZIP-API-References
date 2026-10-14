---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ArchiveSaveOptions 属性。获取或设置用于保存现有 ZIP 存档的加密设置"
type: docs
weight: 60
url: /zh/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

获取或设置用于保存现有 ZIP 存档的加密设置。

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## 备注

不要在常规加密存档的创建中使用此选项，请改用 [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/)。

与具有 ForAllFileEntries 值的 [`DataDescriptorPolicy`](../datadescriptorpolicy/) 不兼容。

## 示例

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### 另请参阅

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


