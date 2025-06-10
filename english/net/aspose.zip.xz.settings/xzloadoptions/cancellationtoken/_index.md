---
title: XzLoadOptions.CancellationToken
second_title: Aspose.ZIP for .NET API Reference
description: XzLoadOptions property. Gets or sets a cancellation token used to cancel the extraction operation
type: docs
weight: 20
url: /net/aspose.zip.xz.settings/xzloadoptions/cancellationtoken/
---
## XzLoadOptions.CancellationToken property

Gets or sets a cancellation token used to cancel the extraction operation.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarks

This property exists for .NET Framework 4.0 and above.

## Examples

Cancel lzip archive extraction after a certain time.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new XzArchive("big.xz", new XzLoadOptions() { CancellationToken = cts.Token }))
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

Using with `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new XzLoadOptions() { CancellationToken = cts.Token };
    using (var a = XzArchive("big.xz", loadOptions))
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

Cancellation mostly results in some data not being extracted.

### See Also

* class [XzLoadOptions](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzloadoptions/)
* assembly [Aspose.Zip](../../../)


