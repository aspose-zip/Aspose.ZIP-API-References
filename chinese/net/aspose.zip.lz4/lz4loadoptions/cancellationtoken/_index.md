---
title: "Lz4LoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Lz4LoadOptions 属性。获取或设置用于取消提取操作的取消令牌。"
type: docs
weight: 20
url: /zh/net/aspose.zip.lz4/lz4loadoptions/cancellationtoken/
---
## Lz4LoadOptions.CancellationToken property

获取或设置用于取消提取操作的取消令牌。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 备注

此属性适用于 .NET Framework 4.0 及以上版本。

## 示例

在一定时间后取消 lz4 归档提取。

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

与 `Task` 一起使用

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

取消操作通常会导致部分数据未被提取。

### 另请参阅

* class [Lz4LoadOptions](../)
* namespace [Aspose.Zip.Lz4](../../lz4loadoptions/)
* assembly [Aspose.Zip](../../../)


