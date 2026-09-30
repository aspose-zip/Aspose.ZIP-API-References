---
title: "ParallelOptions クラス"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Saving.ParallelOptions クラス。並列圧縮のオプション"
type: docs
weight: 990
url: /ja/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

並列圧縮のオプション。

```csharp
public class ParallelOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | デフォルト コンストラクタです。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | ディスクへのスワップなしで圧縮エントリを収容できるメモリ見積もり（メガバイト）を取得または設定します。この値は、[`ParallelCompressInMemory`](./parallelcompressinmemory/) 設定が自動モードの場合にのみ意味があります。 |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | 並列アプローチの使用方法を示す値を取得または設定します。 |

## 備考

これらのオプションは、複数の CPU コアによる同時圧縮を管理します。

## 例

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = ParallelCompressionMode.Auto, AvailableMemorySize = 4000 } });
}
```

### 関連項目

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


