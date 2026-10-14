---
title: "AlzArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AlzArchiveLoadOptions 属性。获取或设置用于取消提取操作的取消令牌"
type: docs
weight: 20
url: /zh/net/aspose.zip.alz/alzarchiveloadoptions/cancellationtoken/
---
## AlzArchiveLoadOptions.CancellationToken property

获取或设置用于取消提取操作的取消令牌。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 备注

此属性适用于 .NET Framework 4.0 及以上版本。

## 示例

在一定时间后取消 ALZ 存档提取。

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new AlzArchive("big.alz", new AlzArchiveLoadOptions() { CancellationToken = cts.Token }))
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

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


