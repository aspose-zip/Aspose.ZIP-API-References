---
title: "AlzArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AlzArchiveLoadOptions egenskap. Hämtar eller anger en avbokningstoken som används för att avbryta extraktionsoperationen"
type: docs
weight: 20
url: /sv/net/aspose.zip.alz/alzarchiveloadoptions/cancellationtoken/
---
## AlzArchiveLoadOptions.CancellationToken property

Hämtar eller anger en avbokningstoken som används för att avbryta extraktionsoperationen.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Anmärkningar

Denna egenskap finns för .NET Framework 4.0 och senare.

## Exempel

Avbryt ALZ-arkivextraktion efter en viss tid.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new AlzArchive("big.alz", new AlzArchiveLoadOptions() { CancellationToken = cts.Token }))
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

### Se även

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


