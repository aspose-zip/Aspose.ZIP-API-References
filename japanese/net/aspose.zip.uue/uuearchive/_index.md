---
title: "クラス UueArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Uue.UueArchive クラス。このクラスは uuencode されたファイルを表します"
type: docs
weight: 1310
url: /ja/net/aspose.zip.uue/uuearchive/
---
## UueArchive class

このクラスは uuencoded ファイルを表します。

```csharp
public class UueArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [UueArchive](uuearchive/#constructor)() | `UueArchive` クラスの新しいインスタンスを初期化し、エンコード用に準備します。 |
| [UueArchive](uuearchive/#constructor_1)(Stream) | `UueArchive` クラスの新しいインスタンスを初期化し、デコード用に準備します。 |
| [UueArchive](uuearchive/#constructor_2)(string) | `UueArchive` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Name](../../aspose.zip.uue/uuearchive/name/) { get; } | 元のファイル名。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.uue/uuearchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.uue/uuearchive/extract/#extract_1)(Stream) | 提供されたストリームへアーカイブを抽出します。 |
| [Extract](../../aspose.zip.uue/uuearchive/extract/#extract)(string) | パスで指定されたファイルへアーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.uue/uuearchive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Open](../../aspose.zip.uue/uuearchive/open/)() | デコード用にアーカイブを開き、アーカイブ内容のストリームを提供します。 |
| [Save](../../aspose.zip.uue/uuearchive/save/#save)(Stream, UueSaveOptions) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.uue/uuearchive/save/#save_1)(string, UueSaveOptions) | 提供された宛先ファイルにアーカイブを保存します。 |
| [SetSource](../../aspose.zip.uue/uuearchive/setsource/#setsource)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.uue/uuearchive/setsource/#setsource_1)(Stream) | アーカイブ内でエンコードされる内容を設定します。 |
| [SetSource](../../aspose.zip.uue/uuearchive/setsource/#setsource_2)(string) | アーカイブ内でエンコードされる内容を設定します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Uue](../../aspose.zip.uue/)
* assembly [Aspose.Zip](../../)


