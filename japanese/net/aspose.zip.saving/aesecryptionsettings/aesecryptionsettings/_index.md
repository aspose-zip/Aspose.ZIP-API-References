---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: AesEcryptionSettings コンストラクタ. の新しいインスタンスを初期化しますAesEcryptionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

の新しいインスタンスを初期化します[`AesEcryptionSettings`](../)class.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| password | String | 暗号化または復号化のためのパスワード。 |
| method | EncryptionMethod | 暗号のブロックサイズを示すアルゴリズムオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| NotSupportedException | *method*の 1 つではありませんAES128、AES192 、 またAES256. |

### 例

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### 関連項目

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../aesecryptionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

の新しいインスタンスを初期化します[`AesEcryptionSettings`](../)パスワードなしのクラス.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| method | EncryptionMethod | 暗号のブロックサイズを示すアルゴリズムオプション。 |

### 関連項目

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../aesecryptionsettings/)
* 組み立て [Aspose.Zip](../../../)


