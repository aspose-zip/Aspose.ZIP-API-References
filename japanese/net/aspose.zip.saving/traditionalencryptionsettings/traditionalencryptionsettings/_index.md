---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: TraditionalEncryptionSettings コンストラクタ. の新しいインスタンスを初期化しますTraditionalEncryptionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

の新しいインスタンスを初期化します[`TraditionalEncryptionSettings`](../)class.

```csharp
public TraditionalEncryptionSettings(string password)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| password | String | 暗号化用のパスワード。 |

### 例

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [TraditionalEncryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

の新しいインスタンスを初期化します[`TraditionalEncryptionSettings`](../)ユーザー定義のエンコーディングを持つクラス.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| password | String | 暗号化用のパスワード。 |
| encoding | Encoding | パスワード文字のエンコード。 |

### 備考

このコンストラクターの使用は推奨されません。エンコーディングを設定すると、標準と矛盾し、互換性のないアーカイブが生成される場合があります。

### 例

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [TraditionalEncryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

の新しいインスタンスを初期化します[`TraditionalEncryptionSettings`](../)パスワードなしのクラス.

```csharp
public TraditionalEncryptionSettings()
```

### 関連項目

* class [TraditionalEncryptionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 組み立て [Aspose.Zip](../../../)


