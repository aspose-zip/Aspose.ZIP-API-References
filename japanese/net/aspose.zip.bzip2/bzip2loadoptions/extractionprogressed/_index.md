---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Bzip2LoadOptions イベント。いくつかのバイトが抽出されたときに発生するイベントです。"
type: docs
weight: 30
url: /ja/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

バイトが抽出されたときに呼び出されるイベントです。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 備考

イベントの送信者は抽出が進行中の [`Bzip2Archive`](../../bzip2archive/) インスタンスです。[`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) は抽出後のバイト数です。

## 例

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


