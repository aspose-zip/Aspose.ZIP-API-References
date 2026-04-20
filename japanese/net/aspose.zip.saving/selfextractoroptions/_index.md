---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Saving.SelfExtractorOptions クラス. 自己解凍型の実行可能アーカイブを作成するためのオプション
type: docs
weight: 500
url: /ja/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

自己解凍型の実行可能アーカイブを作成するためのオプション。

```csharp
public class SelfExtractorOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | 抽出時に抽出ウィンドウを閉じる必要があるかどうかを示す値を取得または設定します。 |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | エクストラクターのウィンドウのタイトルを取得または設定します。 |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | アーカイブの抽出が完了した後に実行されるプログラムを取得または設定します。 |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | 抽出アプリケーションのメイン ウィンドウのタイトル アイコンへのパスを取得または設定します。 |

### 備考

従量制ライセンスでは自己解凍アーカイブを構成できません:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### 例

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### 関連項目

* 名前空間 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 組み立て [Aspose.Zip](../../)


