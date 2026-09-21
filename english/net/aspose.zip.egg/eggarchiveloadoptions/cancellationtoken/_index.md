---
title: EggArchiveLoadOptions.CancellationToken
second_title: Aspose.ZIP for .NET API Reference
description: EggArchiveLoadOptions property. Gets or sets a cancellation token used to cancel the extraction operation
type: docs
weight: 20
url: /net/aspose.zip.egg/eggarchiveloadoptions/cancellationtoken/
---
## EggArchiveLoadOptions.CancellationToken property

Gets or sets a cancellation token used to cancel the extraction operation.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarks

This property exists for .NET Framework 4.0 and above.

## Examples

Cancel EGG archive extraction after a certain time.

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

### See Also

* class [EggArchiveLoadOptions](../)
* namespace [Aspose.Zip.Egg](../../eggarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


