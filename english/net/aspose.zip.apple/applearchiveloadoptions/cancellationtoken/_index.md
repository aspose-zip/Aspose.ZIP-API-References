---
title: AppleArchiveLoadOptions.CancellationToken
second_title: Aspose.ZIP for .NET API Reference
description: AppleArchiveLoadOptions property. Gets or sets a cancellation token used to cancel the extraction operation
type: docs
weight: 20
url: /net/aspose.zip.apple/applearchiveloadoptions/cancellationtoken/
---
## AppleArchiveLoadOptions.CancellationToken property

Gets or sets a cancellation token used to cancel the extraction operation.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarks

This property exists for .NET Framework 4.0 and above.

## Examples

Cancel Apple Archive extraction after a certain time.

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

Using with `Task`

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

Cancellation mostly results in some data not being extracted.

### See Also

* class [AppleArchiveLoadOptions](../)
* namespace [Aspose.Zip.Apple](../../applearchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


