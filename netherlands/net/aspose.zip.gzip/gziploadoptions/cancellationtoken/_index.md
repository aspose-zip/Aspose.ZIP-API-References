---
title: "GzipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "GzipLoadOptions property. Haalt de waarde op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑operatie te annuleren"
type: docs
weight: 20
url: /nl/net/aspose.zip.gzip/gziploadoptions/cancellationtoken/
---
## GzipLoadOptions.CancellationToken property

Haalt op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑bewerking te annuleren.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Opmerkingen

Deze eigenschap bestaat voor .NET Framework 4.0 en hoger.

## Voorbeelden

Annuleer de extractie van het gzip‑archief na een bepaalde tijd.

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

Gebruik met `Task`

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

Annulering resulteert meestal in het niet extraheren van sommige gegevens.

### Zie ook

* class [GzipLoadOptions](../)
* namespace [Aspose.Zip.Gzip](../../gziploadoptions/)
* assembly [Aspose.Zip](../../../)


