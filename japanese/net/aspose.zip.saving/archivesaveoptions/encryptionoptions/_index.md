---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveSaveOptions プロパティ。既存の ZIP アーカイブを保存するための暗号化設定を取得または設定します。"
type: docs
weight: 60
url: /ja/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

既存の ZIP アーカイブを保存するための暗号化設定を取得または設定します。

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## 備考

暗号化されたアーカイブの通常の作成にはこのオプションを使用しないでください。代わりに [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) を使用してください。

値 ForAllFileEntries を持つ場合、[`DataDescriptorPolicy`](../datadescriptorpolicy/) と互換性がありません。

## 例

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### 関連項目

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


