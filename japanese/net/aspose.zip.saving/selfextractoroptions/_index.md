---
title: "クラス SelfExtractorOptions"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Saving.SelfExtractorOptions クラス。自己抽出実行可能アーカイブの作成オプション"
type: docs
weight: 1000
url: /ja/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

自己解凍実行可能アーカイブの作成オプション。

```csharp
public class SelfExtractorOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | デフォルト コンストラクタです。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | 抽出時にエクストラクタウィンドウを閉じるかどうかを示す値を取得または設定します。 |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | エクストラクタウィンドウのタイトルを取得または設定します。 |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | アーカイブ抽出が完了した後に実行されるプログラムを取得または設定します。 |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | エクストラクタアプリケーションのメインウィンドウ用タイトルアイコンへのパスを取得または設定します。 |

## 例

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictogram.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### 関連項目

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


