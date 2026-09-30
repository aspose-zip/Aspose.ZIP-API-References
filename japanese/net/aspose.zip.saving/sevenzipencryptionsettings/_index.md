---
title: "クラス SevenZipEncryptionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Saving.SevenZipEncryptionSettings クラス。複数の 7z 暗号化方式の設定の基底クラスです。"
type: docs
weight: 1060
url: /ja/net/aspose.zip.saving/sevenzipencryptionsettings/
---
## SevenZipEncryptionSettings class

複数の 7z 暗号化方式の設定用の基底クラス。

```csharp
public abstract class SevenZipEncryptionSettings
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [EncryptHeader](../../aspose.zip.saving/sevenzipencryptionsettings/encryptheader/) { get; set; } | ヘッダー暗号化を示す値を取得または設定します。 |
| [Password](../../aspose.zip.saving/sevenzipencryptionsettings/password/) { get; set; } | 暗号化または復号化のためのパスワードを取得または設定します。 |

## 備考

AES-256 は 7z アーカイブで唯一可能な暗号化方式です。そのため、[`SevenZipAESEncryptionSettings`](../sevenzipaesencryptionsettings/) が唯一の実装です。

### 関連項目

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


