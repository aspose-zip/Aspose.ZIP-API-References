---
title: "クラス AppleArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Apple.AppleArchive クラス。このクラスは Apple Archive の .aar ファイルを表します。Apple Archive ファイルを作成するために使用します。"
type: docs
weight: 60
url: /ja/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

このクラスは Apple アーカイブ (.aar) ファイルを表します。Apple アーカイブ ファイルを作成するために使用します。

```csharp
public class AppleArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | `AppleArchive` クラスの新しいインスタンスを、作成されたエントリで使用される設定とともに初期化します。 |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | `AppleArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | `AppleArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | アーカイブを構成するエントリを取得します。 |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | アーカイブがソリッド圧縮を使用しているかどうかを示す値を取得します。ソリッドモードでは、すべてのエントリデータが単一のストリームとして圧縮され、個々のエントリ抽出は利用できません。代わりに [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) を使用してください。 |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | 新しく作成されたエントリで使用される設定を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | 提供された宛先ファイルにアーカイブを保存します。 |

## 備考

Apple と Apple Archive は Apple Inc. の商標です。

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


