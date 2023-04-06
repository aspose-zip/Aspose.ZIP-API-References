---
title: Class Bzip2Archive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Bzip2.Bzip2Archive クラス. このクラスはbzip2 アーカイブ ファイルを表しますこれを使用してbzip2 アーカイブを作成または抽出します
type: docs
weight: 100
url: /ja/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

このクラスは、bzip2 アーカイブ ファイルを表します。これを使用して、bzip2 アーカイブを作成または抽出します。

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | の新しいインスタンスを初期化します`Bzip2Archive`圧縮用に準備されたクラス. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream) | の新しいインスタンスを初期化します`Bzip2Archive`解凍用に準備されたクラス. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string) | の新しいインスタンスを初期化します`Bzip2Archive`解凍用に準備されたクラス. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/)(Stream) | 提供されたストリームにアーカイブを抽出します。 |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | 抽出のためにアーカイブを開き、アーカイブ コンテンツを含むストリームを提供します。 |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | 提供されたストリームにアーカイブを保存します。 |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | 指定された宛先ファイルにアーカイブを保存します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | アーカイブ内で圧縮するコンテンツを設定します。 |

### 備考

bzip2 は、Burrows-Wheeler ブロック ソート テキスト圧縮アルゴリズムとハフマン コーディングを使用してファイルを圧縮します。詳細: https://en.wikipedia.org/wiki/Bzip2

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 名前空間 [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* 組み立て [Aspose.Zip](../../)


