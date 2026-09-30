---
title: "TraditionalEncryptionSettings.TraditionalEncryptionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TraditionalEncryptionSettings コンストラクタ。TraditionalEncryptionSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

[`TraditionalEncryptionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public TraditionalEncryptionSettings(string password)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| password | String | 暗号化用パスワード。 |

## 例

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

ユーザー定義のエンコーディングを使用して、[`TraditionalEncryptionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| password | String | 暗号化用パスワード。 |
| encoding | エンコーディング | パスワード文字のエンコーディング。 |

## 備考

このコンストラクタの使用は推奨されません。エンコーディングを設定すると標準に矛盾し、互換性のないアーカイブが生成される可能性があります。

## 例

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

パスワードなしで[`TraditionalEncryptionSettings`](../)クラスの新しいインスタンスを初期化します。

```csharp
public TraditionalEncryptionSettings()
```

### 関連項目

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)


