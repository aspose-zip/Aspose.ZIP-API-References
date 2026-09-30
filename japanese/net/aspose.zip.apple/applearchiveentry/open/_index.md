---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AppleArchiveEntry メソッド。エントリを抽出用に開き、エントリ内容を含むストリームを提供します"
type: docs
weight: 60
url: /ja/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

エントリを抽出用に開き、エントリの内容を含むストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

抽出されたエントリ データを含む読み取り可能なストリームです。

### 例外

| 例外 | 条件 |
| --- | --- |
| NotSupportedException | エントリはソリッド Apple アーカイブに属しているか、サポートされていない圧縮方式を使用しています。 |
| InvalidDataException | エントリに保存されているチェックサムまたはダイジェストが抽出データと一致しません。 |
| InvalidOperationException | エントリは合成用に準備されたアーカイブに属しているか、シーク不可のアーカイブ ストリームからエントリ データを開くことができません。 |
| ObjectDisposedException | ソース ストリームは破棄されました。 |
| IOException | I/O エラーが発生しました。 |

## 備考

返されたストリームから読み取って元のエントリ内容を取得してください。アーカイブにチェックサム フィールドが含まれている場合、返されたストリームを読み取る間にチェックサムが検証されます。

### 関連項目

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


