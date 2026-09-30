---
title: "SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipAESEncryptionSettings コンストラクタ。SevenZipAESEncryptionSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

[`SevenZipAESEncryptionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| password | String | 暗号化または復号化のためのパスワードです。 |

## 例

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 関連項目

* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

外部暗号を使用して、[`SevenZipAESEncryptionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 暗号 | SevenZipCipher | カスタム AES 実装。 |

## 例

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
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)


