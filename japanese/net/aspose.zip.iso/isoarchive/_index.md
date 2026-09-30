---
title: "クラス IsoArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Iso.IsoArchive クラス。ISO 9660 アーカイブを表します。"
type: docs
weight: 570
url: /ja/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

ISO アーカイブ (ISO 9660) を表します。

```csharp
public sealed class IsoArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | 新しい `IsoArchive` クラスのインスタンスを初期化し、新しいファイルやディレクトリを追加するための空の ISO アーカイブを作成します。 |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | 新しい `IsoArchive` クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | 新しい `IsoArchive` クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | アーカイブを構成する [`IsoEntry`](../isoentry/) 型のエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | ISO イメージにディレクトリを追加します。 |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | ISO イメージにファイルを追加します。 |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | ISO イメージにファイルを追加します。 |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | ISO イメージにファイルを追加します。 |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | すべてのエントリを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | ISO イメージを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | ISO イメージを指定されたパスに保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


