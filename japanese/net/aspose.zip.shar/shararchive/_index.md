---
title: Class SharArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Shar.SharArchive クラス. このクラスはshar アーカイブ ファイルを表します
type: docs
weight: 700
url: /ja/net/aspose.zip.shar/shararchive/
---
## SharArchive class

このクラスは、shar アーカイブ ファイルを表します。

```csharp
public class SharArchive : IDisposable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | の新しいインスタンスを初期化します`SharArchive`class. |
| [SharArchive](shararchive/#constructor_1)(string) |  |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | のエントリを取得します[`SharEntry`](../sharentry/)アーカイブを構成するタイプ. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | インデックスによってエントリ リストからエントリを削除します。 |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | 提供されたストリームにアーカイブを保存します。 |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | 指定された宛先ファイルにアーカイブを保存します。 |

### 関連項目

* 名前空間 [Aspose.Zip.Shar](../../aspose.zip.shar/)
* 組み立て [Aspose.Zip](../../)


