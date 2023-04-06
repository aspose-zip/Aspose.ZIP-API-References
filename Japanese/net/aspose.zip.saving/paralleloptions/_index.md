---
title: Class ParallelOptions
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Saving.ParallelOptions クラス. 並列圧縮のオプション
type: docs
weight: 490
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
| [ParallelOptions](paralleloptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | ディスクにスワップせずに圧縮されたエントリに対応するために使用できるメガバイト単位のメモリ見積もりを取得または設定します。 この値は、次の場合にのみ意味があります[`ParallelCompressInMemory`](./parallelcompressinmemory/)設定はAutomode. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | 並列アプローチの使用方法を示す値を取得または設定します。 |

### 備考

これらのオプションは、複数の CPU コアによる同時圧縮を管理します。

### 例

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### 関連項目

* 名前空間 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 組み立て [Aspose.Zip](../../)


