---
title: "ParallelOptions.AvailableMemorySize"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ParallelOptions プロパティ。ディスクへのスワップなしで圧縮エントリを収容できるメモリの推定サイズ（メガバイト）を取得または設定します。この値は ParallelCompressInMemory 設定が Auto モードの場合にのみ意味があります。"
type: docs
weight: 20
url: /ja/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

ディスクへのスワップなしで圧縮エントリを収容できるメモリの推定サイズ（メガバイト）を取得または設定します。この値は[`ParallelCompressInMemory`](../parallelcompressinmemory/)設定が Auto モードの場合にのみ意味があります。

```csharp
public int AvailableMemorySize { get; set; }
```

## 備考

この値は、他のエントリと並列で圧縮できるエントリの最大サイズを計算するために使用されます。計算された閾値を超えるすべてのエントリは順次圧縮されます。`AvailableMemorySize` プロパティは、空き RAM と同等かそれ以上の大きさに設定しても安全です。デフォルトでは、CPU コアあたり少なくとも 200MB のメモリがあると想定しています。

### 関連項目

* class [ParallelOptions](../)
* namespace [Aspose.Zip.Saving](../../paralleloptions/)
* assembly [Aspose.Zip](../../../)


