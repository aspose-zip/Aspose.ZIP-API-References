---
title: "SevenZipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "SevenZipLoadOptions-Eigenschaft. Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird"
type: docs
weight: 20
url: /de/net/aspose.zip.sevenzip/sevenziploadoptions/cancellationtoken/
---
## SevenZipLoadOptions.CancellationToken property

Liest oder setzt ein Abbruch-Token, das zum Abbrechen des Extraktionsvorgangs verwendet wird.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Hinweise

Diese Eigenschaft existiert für .NET Framework 4.0 und höher.

## Beispiele

Brechen Sie die 7Z-Archivextraktion nach einer bestimmten Zeit ab.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new SevenZipArchive("big.7z", new SevenZipLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new SevenZipLoadOptions() { CancellationToken = cts.Token };
    using (var a = new SevenZipArchive("big.7z", loadOptions))
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

* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


