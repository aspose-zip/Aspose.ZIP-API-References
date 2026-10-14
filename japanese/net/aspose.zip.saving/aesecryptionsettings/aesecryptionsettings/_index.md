---
title: "AesEcryptionSettings.AesEcryptionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AesEcryptionSettings コンストラクタ。AesEcryptionSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

[`AesEcryptionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| password | String | 暗号化または復号化のためのパスワードです。 |
| method | EncryptionMethod | 暗号のブロックサイズを示すアルゴリズムオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| NotSupportedException | *method* は AES128、AES192、または AES256 のいずれでもありません。 |

## 例

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
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

パスワードなしで、[`AesEcryptionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| method | EncryptionMethod | 暗号のブロックサイズを示すアルゴリズムオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| NotSupportedException | *method* は AES128、AES192、または AES256 のいずれでもありません。 |

### 関連項目

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)


