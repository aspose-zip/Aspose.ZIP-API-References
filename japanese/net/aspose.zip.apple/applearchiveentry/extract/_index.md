---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AppleArchiveEntry メソッド。指定されたパスでエントリをファイルシステムに抽出します"
type: docs
weight: 50
url: /ja/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

エントリを提供されたパスでファイルシステムに抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパスです。ファイルが既に存在する場合、上書きされます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidDataException | エントリに保存されているチェックサムまたはダイジェストが抽出データと一致しません。 |
| InvalidOperationException | エントリは合成用に準備されたアーカイブに属しているか、シーク不可のアーカイブ ストリームからエントリ データを開くことができません。 |
| NotSupportedException | エントリはソリッド Apple アーカイブに属しているか、サポートされていない圧縮方式を使用しています。 |
| ObjectDisposedException | ソース ストリームは破棄されました。 |
| IOException | I/O エラーが発生しました。 |

### 関連項目

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

エントリを提供されたストリームに抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *destination* は `null` です。 |
| ArgumentException | *destination* は書き込みをサポートしていません。 |
| InvalidDataException | エントリに保存されているチェックサムまたはダイジェストが抽出データと一致しません。 |
| InvalidOperationException | エントリは合成用に準備されたアーカイブに属しているか、シーク不可のアーカイブ ストリームからエントリ データを開くことができません。 |
| NotSupportedException | エントリはソリッド Apple アーカイブに属しているか、サポートされていない圧縮方式を使用しています。 |
| ObjectDisposedException | ソース ストリームは破棄されました。 |
| IOException | I/O エラーが発生しました。 |

### 関連項目

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


