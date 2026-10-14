---
title: "Lz4LoadOptions.CancellationToken"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Lz4LoadOptions プロパティ。抽出操作をキャンセルするために使用されるキャンセルトークンを取得または設定します。"
type: docs
weight: 20
url: /ja/net/aspose.zip.lz4/lz4loadoptions/cancellationtoken/
---
## Lz4LoadOptions.CancellationToken property

抽出操作をキャンセルするために使用されるキャンセルトークンを取得または設定します。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 備考

このプロパティは .NET Framework 4.0 以降で使用できます。

## 例

一定時間後に lz4 アーカイブの抽出をキャンセルします。

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new Lz4Archive("big.lz4", new Lz4LoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Extract("data.bin");
        }
        catch(OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

`Task` と併用する

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new Lz4LoadOptions() { CancellationToken = cts.Token };
    using (var a = Lz4Archive("big.lz4", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(Task antecedent)
{
     if (antecedent.IsCanceled)
     {
         Console.WriteLine("Extraction was cancelled after 60 seconds");
     }

     cts.Dispose();
});
```

キャンセルにより、主に一部のデータが抽出されないことがあります。

### 関連項目

* class [Lz4LoadOptions](../)
* namespace [Aspose.Zip.Lz4](../../lz4loadoptions/)
* assembly [Aspose.Zip](../../../)


