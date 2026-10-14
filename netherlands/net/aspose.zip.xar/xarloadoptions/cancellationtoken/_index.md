---
title: "XarLoadOptions.CancellationToken"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarLoadOptions-eigenschap. Haalt op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑operatie te annuleren."
type: docs
weight: 20
url: /nl/net/aspose.zip.xar/xarloadoptions/cancellationtoken/
---
## XarLoadOptions.CancellationToken property

Haalt op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑bewerking te annuleren.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Opmerkingen

Deze eigenschap bestaat voor .NET Framework 4.0 en hoger.

## Voorbeelden

Annuleer XAR-archiefextractie na een bepaalde tijd.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new XarArchive("big.xar", new XarLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             (XarFileEntry)(a.Entries.First()).Extract("data.bin");
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
    var loadOptions = new XarLoadOptions() { CancellationToken = cts.Token };
    using (var a = new XarArchive("big.xar", loadOptions))
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

* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


