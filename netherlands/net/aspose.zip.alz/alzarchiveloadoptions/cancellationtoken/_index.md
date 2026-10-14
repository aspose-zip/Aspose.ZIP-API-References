---
title: "AlzArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AlzArchiveLoadOptions property. Haalt op of stelt een annulerings‑token in dat wordt gebruikt om de extractie‑bewerking te annuleren"
type: docs
weight: 20
url: /nl/net/aspose.zip.alz/alzarchiveloadoptions/cancellationtoken/
---
## AlzArchiveLoadOptions.CancellationToken property

Haalt op of stelt een annulerings-token in dat wordt gebruikt om de extractie‑bewerking te annuleren.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Opmerkingen

Deze eigenschap bestaat voor .NET Framework 4.0 en hoger.

## Voorbeelden

Annuleer de extractie van het ALZ‑archief na een bepaalde tijd.

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

### Zie ook

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


