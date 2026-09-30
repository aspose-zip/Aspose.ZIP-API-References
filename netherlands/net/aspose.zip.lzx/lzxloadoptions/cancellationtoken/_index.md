---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "LzxLoadOptions eigenschap. Haalt een annulerings-token op of stelt het in dat wordt gebruikt om de extractieoperatie te annuleren"
type: docs
weight: 20
url: /nl/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Haalt op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑bewerking te annuleren.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Opmerkingen

Deze eigenschap bestaat voor .NET Framework 4.0 en hoger.

## Voorbeelden

Annuleer Lzx-archiefextractie na een bepaalde tijd.

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

Gebruik met `Task`

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

Annulering resulteert meestal in het niet extraheren van sommige gegevens.

### Zie ook

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


