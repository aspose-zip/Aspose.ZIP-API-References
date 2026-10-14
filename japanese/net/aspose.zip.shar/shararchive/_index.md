---
title: "クラス SharArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Shar.SharArchive クラス。このクラスは shar アーカイブ ファイルを表します。"
type: docs
weight: 1240
url: /ja/net/aspose.zip.shar/shararchive/
---
## SharArchive class

このクラスは shar アーカイブ ファイルを表します。

```csharp
public class SharArchive : IDisposable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | `SharArchive` クラスの新しいインスタンスを初期化します。 |
| [SharArchive](shararchive/#constructor_1)(string) | 解凍用に準備された `SharArchive` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | アーカイブを構成する [`SharEntry`](../sharentry/) 型のエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | インデックスでエントリリストからエントリを削除します。 |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | 提供された宛先ファイルにアーカイブを保存します。 |

### 関連項目

* namespace [Aspose.Zip.Shar](../../aspose.zip.shar/)
* assembly [Aspose.Zip](../../)


