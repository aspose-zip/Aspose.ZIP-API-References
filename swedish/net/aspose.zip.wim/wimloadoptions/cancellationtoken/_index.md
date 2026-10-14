---
title: "WimLoadOptions.CancellationToken"
second_title: "Aspose.ZIP för .NET API-referens"
description: "WimLoadOptions-egenskap. Hämtar eller anger en avbokningstoken som används för att avbryta extraheringsoperationen"
type: docs
weight: 20
url: /sv/net/aspose.zip.wim/wimloadoptions/cancellationtoken/
---
## WimLoadOptions.CancellationToken property

Hämtar eller anger en avbokningstoken som används för att avbryta extraktionsoperationen.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Anmärkningar

Denna egenskap finns för .NET Framework 4.0 och senare.

## Exempel

Avbryt WIM-arkivextraktion efter en viss tid.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new WimArchive("big.wim", new WimLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
            a.Images[0].AllEntries.OfType<WimFileEntry>().First().Extract("data.bin");
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
    var loadOptions = new WimLoadOptions() { CancellationToken = cts.Token };
    using (var a = WimArchive("big.wim", loadOptions))
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

* class [WimLoadOptions](../)
* namespace [Aspose.Zip.Wim](../../wimloadoptions/)
* assembly [Aspose.Zip](../../../)


