---
title: "CabLoadOptions.CancellationToken"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CabLoadOptions-egenskap. Hämtar eller anger en avbokningstoken som används för att avbryta extraktionsoperationen"
type: docs
weight: 20
url: /sv/net/aspose.zip.cab/cabloadoptions/cancellationtoken/
---
## CabLoadOptions.CancellationToken property

Hämtar eller anger en avbokningstoken som används för att avbryta extraktionsoperationen.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Anmärkningar

Denna egenskap finns för .NET Framework 4.0 och senare.

## Exempel

Avbryt CAB-arkivextraktion efter en viss tid.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new CabArchive("big.cab", new CabLoadOptions() { CancellationToken = cts.Token }))
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

Användning med `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new CabLoadOptions() { CancellationToken = cts.Token };
    using (var a = new CabArchive("big.cab", loadOptions))
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

Avbrytning resulterar oftast i att vissa data inte extraheras.

### Se även

* class [CabLoadOptions](../)
* namespace [Aspose.Zip.Cab](../../cabloadoptions/)
* assembly [Aspose.Zip](../../../)


