---
title: "EggArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "EggArchiveLoadOptions-Eigenschaft. Gibt ein Abbruch-Token zurück oder legt es fest, das zum Abbrechen des Extraktionsvorgangs verwendet wird"
type: docs
weight: 20
url: /de/net/aspose.zip.egg/eggarchiveloadoptions/cancellationtoken/
---
## EggArchiveLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

Bricht die EGG-Archiv-Extraktion nach einer bestimmten Zeit ab.

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

### Siehe auch

* class [EggArchiveLoadOptions](../)
* namespace [Aspose.Zip.Egg](../../eggarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


