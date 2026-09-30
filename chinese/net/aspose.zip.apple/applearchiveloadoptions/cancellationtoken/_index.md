---
title: "AppleArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AppleArchiveLoadOptions 属性。获取或设置用于取消提取操作的取消令牌"
type: docs
weight: 20
url: /zh/net/aspose.zip.apple/applearchiveloadoptions/cancellationtoken/
---
## AppleArchiveLoadOptions.CancellationToken property

获取或设置用于取消提取操作的取消令牌。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 备注

此属性适用于 .NET Framework 4.0 及以上版本。

## 示例

在一定时间后取消 Apple Archive 的提取。

```csharp
using (System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource())
{
    cts.CancelAfter(System.TimeSpan.FromSeconds(60)); 
    using (var a = new AppleArchive("big.aar", new AppleArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.ExtractToDirectory("destination");
        }
        catch(System.OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

与 `Task` 一起使用

```csharp
System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource();
cts.CancelAfter(System.TimeSpan.FromSeconds(60));
System.Threading.Tasks.Task t = System.Threading.Tasks.Task.Run(delegate()
{
    var loadOptions = new AppleArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new AppleArchive("big.aar", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(System.Threading.Tasks.Task antecedent)
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

* class [AppleArchiveLoadOptions](../)
* namespace [Aspose.Zip.Apple](../../applearchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


