---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZstandardLoadOptions イベント。いくつかのバイトが抽出されたときに呼び出されるデリゲートを取得または設定します"
type: docs
weight: 30
url: /ja/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

バイトが抽出されたときに呼び出されるデリゲートを取得または設定します。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 備考

イベントの送信者は抽出が進行している [`ZstandardArchive`](../../zstandardarchive/) インスタンスです。

## 例

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


