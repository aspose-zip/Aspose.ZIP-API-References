---
title: "ArjLoadOptions.CancellationToken"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ArjLoadOptions‑eigenschap. Haalt een annulerings‑token op of stelt deze in, gebruikt om de extractie‑operatie te annuleren."
type: docs
weight: 20
url: /nl/net/aspose.zip.arj/arjloadoptions/cancellationtoken/
---
## ArjLoadOptions.CancellationToken property

Haalt op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑bewerking te annuleren.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Opmerkingen

Deze eigenschap bestaat voor .NET Framework 4.0 en hoger.

## Voorbeelden

Annuleer ARJ‑archiefextractie na een bepaalde tijd.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new ArjArchive("big.arj", new ArjLoadOptions() { CancellationToken = cts.Token }))
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
    ArjLoadOptions loadOptions = new ArjLoadOptions() { CancellationToken = cts.Token };
    using (ArjArchive a = new ArjArchive("big.arj", loadOptions))
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

* class [ArjLoadOptions](../)
* namespace [Aspose.Zip.Arj](../../arjloadoptions/)
* assembly [Aspose.Zip](../../../)


