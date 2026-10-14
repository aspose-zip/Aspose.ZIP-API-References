---
title: "AppleArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AppleArchiveLoadOptions-Eigenschaft. Gibt ein CancellationToken zurück oder legt es fest, das zum Abbrechen des Extraktionsvorgangs verwendet wird"
type: docs
weight: 20
url: /de/net/aspose.zip.apple/applearchiveloadoptions/cancellationtoken/
---
## AppleArchiveLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

Brechen Sie die Apple-Archiv-Extraktion nach einer bestimmten Zeit ab.

```csharp
using (System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource())
{
    cts.CancelAfter(System.TimeSpan.FromSeconds(60)); 
    using (var a = new AppleArchive("big.aar", new AppleArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.ExtractToDirectory("destination");
        }
        catch(System.OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

Verwendung mit `Task`

```csharp
System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource();
cts.CancelAfter(System.TimeSpan.FromSeconds(60));
System.Threading.Tasks.Task t = System.Threading.Tasks.Task.Run(delegate()
{
    var loadOptions = new AppleArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new AppleArchive("big.aar", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(System.Threading.Tasks.Task antecedent)
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

* class [AppleArchiveLoadOptions](../)
* namespace [Aspose.Zip.Apple](../../applearchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


