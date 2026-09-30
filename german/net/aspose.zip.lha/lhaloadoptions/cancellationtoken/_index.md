---
title: "LhaLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LhaLoadOptions-Eigenschaft. Gibt ein Abbruch-Token zurück oder setzt es, das verwendet wird, um den Extraktionsvorgang abzubrechen"
type: docs
weight: 20
url: /de/net/aspose.zip.lha/lhaloadoptions/cancellationtoken/
---
## LhaLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

LHA-Archivextraktion nach einer bestimmten Zeit abbrechen.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new LhaArchive("big.lha", new LhaLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new LhaLoadOptions() { CancellationToken = cts.Token };
    using (var a = new LhaArchive("big.arj", loadOptions))
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

* class [LhaLoadOptions](../)
* namespace [Aspose.Zip.Lha](../../lhaloadoptions/)
* assembly [Aspose.Zip](../../../)


