---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LzxLoadOptions-Eigenschaft. Gibt ein Abbruch-Token zurück oder legt es fest, das zum Abbrechen des Extraktionsvorgangs verwendet wird"
type: docs
weight: 20
url: /de/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

Breche die Lzx-Archivextraktion nach einer bestimmten Zeit ab.

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

Verwendung mit `Task`

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

Ein Abbruch führt meist dazu, dass einige Daten nicht extrahiert werden.

### Siehe auch

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


