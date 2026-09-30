---
title: "GzipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "GzipLoadOptions-Eigenschaft. Gibt ein CancellationToken zurück oder legt es fest, das zum Abbrechen des Extraktionsvorgangs verwendet wird."
type: docs
weight: 20
url: /de/net/aspose.zip.gzip/gziploadoptions/cancellationtoken/
---
## GzipLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

Gzip-Archivextraktion nach einer bestimmten Zeit abbrechen.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new GzipArchive("big.gz", new GzipLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Extract("data.bin");
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
    var loadOptions = new GzipLoadOptions() { CancellationToken = cts.Token };
    using (var a = GzipArchive("big.gz", loadOptions))
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

* class [GzipLoadOptions](../)
* namespace [Aspose.Zip.Gzip](../../gziploadoptions/)
* assembly [Aspose.Zip](../../../)


