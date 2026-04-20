---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP for .NET API リファレンス
description: ParallelOptions 財産. ディスクにスワップせずに圧縮されたエントリに対応するために使用できるメガバイト単位のメモリ見積もりを取得または設定します この値は次の場合にのみ意味がありますParallelCompressInMemory設定はAutomode.
type: docs
weight: 20
url: /ja/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

ディスクにスワップせずに圧縮されたエントリに対応するために使用できるメガバイト単位のメモリ見積もりを取得または設定します。 この値は、次の場合にのみ意味があります[`ParallelCompressInMemory`](../parallelcompressinmemory/)設定はAutomode.

```csharp
public int AvailableMemorySize { get; set; }
```

### 備考

この値は、他と並行して圧縮できるエントリの最大サイズを計算するために使用されます。計算されたしきい値を超えるすべてのエントリは、順次圧縮されます。 `AvailableMemorySize`プロパティは、空き RAM と同じくらい大きく、さらに大きくなります。デフォルトでは、CPU コアごとに少なくとも 200MB があると想定されています。

### 関連項目

* class [ParallelOptions](../)
* 名前空間 [Aspose.Zip.Saving](../../paralleloptions/)
* 組み立て [Aspose.Zip](../../../)


