---
title: "EggArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API 参考"
description: "EggArchiveLoadOptions 属性。获取或设置用于取消提取操作的取消令牌"
type: docs
weight: 20
url: /zh/net/aspose.zip.egg/eggarchiveloadoptions/cancellationtoken/
---
## EggArchiveLoadOptions.CancellationToken property

获取或设置用于取消提取操作的取消令牌。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 备注

此属性适用于 .NET Framework 4.0 及以上版本。

## 示例

在一定时间后取消 EGG 存档的提取。

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new EggArchive("big.egg", new EggArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
            archive.Entries[0].Extract("data.bin");
        }
        catch(OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

### 另请参阅

* class [EggArchiveLoadOptions](../)
* namespace [Aspose.Zip.Egg](../../eggarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


