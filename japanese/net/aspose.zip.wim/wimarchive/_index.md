---
title: "クラス WimArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Wim.WimArchive クラス。このクラスは wim アーカイブ ファイルを表します。"
type: docs
weight: 1330
url: /ja/net/aspose.zip.wim/wimarchive/
---
## WimArchive class

このクラスは wim アーカイブ ファイルを表します。

```csharp
public class WimArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [WimArchive](wimarchive/#constructor)(Stream, WimLoadOptions) | `WimArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
| [WimArchive](wimarchive/#constructor_1)(string, WimLoadOptions) | `WimArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BootImageIndex](../../aspose.zip.wim/wimarchive/bootimageindex/) { get; } | 起動可能イメージの (0 ベース) インデックスを取得します。 |
| [Entries](../../aspose.zip.wim/wimarchive/entries/) { get; } | アーカイブを構成する [`WimEntry`](../wimentry/) 型のエントリを取得します。 |
| [FileFormatVersion](../../aspose.zip.wim/wimarchive/fileformatversion/) { get; } | ファイル形式のバージョンを取得します。 |
| [Guid](../../aspose.zip.wim/wimarchive/guid/) { get; } | アーカイブの識別 GUID を取得します。 |
| [Images](../../aspose.zip.wim/wimarchive/images/) { get; } | アーカイブを構成する [`WimImage`](../wimimage/) 型のエントリを取得します。 |
| [Manifest](../../aspose.zip.wim/wimarchive/manifest/) { get; } | ファイルと含まれるイメージを記述する埋め込みマニフェストを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.wim/wimarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.wim/wimarchive/extracttodirectory/)(string) | パスで指定されたファイルへアーカイブを抽出します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


