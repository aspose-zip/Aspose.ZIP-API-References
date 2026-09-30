---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LzxLoadOptions 属性。获取或设置用于取消提取操作的取消令牌"
type: docs
weight: 20
url: /zh/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

获取或设置用于取消提取操作的取消令牌。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 备注

此属性适用于 .NET Framework 4.0 及以上版本。

## 示例

在一定时间后取消 Lzx 存档的提取。

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new LzxArchive("big.lzx", new LzxLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Entries[0].Extract("data.bin");
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
    LzxLoadOptions loadOptions = new LzxLoadOptions() { CancellationToken = cts.Token };
    using (LzxArchive a = new LzxArchive("big.lzx", loadOptions))
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

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


