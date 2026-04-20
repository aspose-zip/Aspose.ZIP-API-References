---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipAESEncryptionSettings コンストラクタ. の新しいインスタンスを初期化しますSevenZipAESEncryptionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

の新しいインスタンスを初期化します[`SevenZipAESEncryptionSettings`](../)class.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| password | String | 暗号化または復号化のためのパスワード。 |

### 例

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 関連項目

* class [SevenZipAESEncryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

の新しいインスタンスを初期化します[`SevenZipAESEncryptionSettings`](../)外部暗号を持つクラス.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| cipher | SevenZipCipher | カスタム AES 実装。 |

### 例

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 関連項目

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* 組み立て [Aspose.Zip](../../../)


