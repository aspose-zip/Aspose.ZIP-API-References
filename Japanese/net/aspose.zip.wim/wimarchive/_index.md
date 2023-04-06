---
title: Class WimArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Wim.WimArchive クラス. このクラスは wim アーカイブ ファイルを表します
type: docs
weight: 760
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
| [WimArchive](wimarchive/#constructor)(Stream) | の新しいインスタンスを初期化します`WimArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |
| [WimArchive](wimarchive/#constructor_1)(string) | の新しいインスタンスを初期化します`WimArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BootImageIndex](../../aspose.zip.wim/wimarchive/bootimageindex/) { get; } | ブータブル イメージの (ゼロから始まる) インデックスを取得します。 |
| [FileFormatVersion](../../aspose.zip.wim/wimarchive/fileformatversion/) { get; } | ファイル形式のバージョンを取得します。 |
| [Guid](../../aspose.zip.wim/wimarchive/guid/) { get; } | アーカイブの識別 GUID を取得します。 |
| [Images](../../aspose.zip.wim/wimarchive/images/) { get; } | のエントリを取得します[`WimImage`](../wimimage/)アーカイブを構成するタイプ. |
| [Manifest](../../aspose.zip.wim/wimarchive/manifest/) { get; } | ファイルと含まれている画像を説明する埋め込みマニフェストを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.wim/wimarchive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* 名前空間 [Aspose.Zip.Wim](../../aspose.zip.wim/)
* 組み立て [Aspose.Zip](../../)


