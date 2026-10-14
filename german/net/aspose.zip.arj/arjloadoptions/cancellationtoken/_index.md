---
title: "ArjLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ArjLoadOptions‑Eigenschaft. Gibt ein Abbruch‑Token zurück oder setzt es, das zum Abbrechen des Extraktionsvorgangs verwendet wird"
type: docs
weight: 20
url: /de/net/aspose.zip.arj/arjloadoptions/cancellationtoken/
---
## ArjLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

ARJ‑Archivextraktion nach einer bestimmten Zeit abbrechen.

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

Verwendung mit `Task`

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

Ein Abbruch führt meist dazu, dass einige Daten nicht extrahiert werden.

### Siehe auch

* class [ArjLoadOptions](../)
* namespace [Aspose.Zip.Arj](../../arjloadoptions/)
* assembly [Aspose.Zip](../../../)


