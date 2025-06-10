---
title: GzipLoadOptions.CancellationToken
second_title: Aspose.ZIP for .NET API Reference
description: GzipLoadOptions property. Gets or sets a cancellation token used to cancel the extraction operation
type: docs
weight: 20
url: /net/aspose.zip.gzip/gziploadoptions/cancellationtoken/
---
## GzipLoadOptions.CancellationToken property

Gets or sets a cancellation token used to cancel the extraction operation.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarks

This property exists for .NET Framework 4.0 and above.

## Examples

Cancel gzip archive extraction after a certain time.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new GzipArchive("big.gz", new GzipLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new GzipLoadOptions() { CancellationToken = cts.Token };
    using (var a = GzipArchive("big.gz", loadOptions))
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

* class [GzipLoadOptions](../)
* namespace [Aspose.Zip.Gzip](../../gziploadoptions/)
* assembly [Aspose.Zip](../../../)


