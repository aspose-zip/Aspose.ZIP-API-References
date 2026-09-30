---
title: "クラス Bzip2Archive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Bzip2.Bzip2Archive クラス。このクラスは bzip2 アーカイブファイルを表します。bzip2 アーカイブの作成や抽出に使用します"
type: docs
weight: 280
url: /ja/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

このクラスは bzip2 アーカイブファイルを表します。bzip2 アーカイブの作成または抽出に使用してください。

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | 圧縮用に準備された `Bzip2Archive` クラスの新しいインスタンスを初期化します。 |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream, Bzip2LoadOptions) | 解凍用に準備された `Bzip2Archive` クラスの新しいインスタンスを初期化します。 |
| [Bzip2Archive](bzip2archive/#constructor_2)(string, Bzip2LoadOptions) | 解凍用に準備された `Bzip2Archive` クラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract_1)(Stream) | 提供されたストリームへアーカイブを抽出します。 |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract)(string) | パスで指定されたファイルへアーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.bzip2/bzip2archive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | 抽出用にアーカイブを開き、アーカイブ内容のストリームを提供します。 |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | 提供された宛先ファイルにアーカイブを保存します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | アーカイブ内で圧縮される内容を設定します。 |

## 備考

bzip2 は Burrows-Wheeler ブロックソートテキスト圧縮アルゴリズムとハフマン符号化を使用してファイルを圧縮します。詳細はこちら: https://en.wikipedia.org/wiki/Bzip2

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* assembly [Aspose.Zip](../../)


