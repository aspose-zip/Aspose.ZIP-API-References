---
title: "WimLoadOptions.CancellationToken"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà WimLoadOptions. Ottiene o imposta un token di cancellazione usato per annullare l'operazione di estrazione"
type: docs
weight: 20
url: /it/net/aspose.zip.wim/wimloadoptions/cancellationtoken/
---
## WimLoadOptions.CancellationToken property

Ottiene o imposta un token di cancellazione utilizzato per annullare l'operazione di estrazione.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Osservazioni

Questa proprietà esiste per .NET Framework 4.0 e versioni successive.

## Esempi

Annulla l'estrazione dell'archivio WIM dopo un certo periodo.

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

Utilizzo con `Task`

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

La cancellazione di solito comporta che alcuni dati non vengano estratti.

### Vedi anche

* class [WimLoadOptions](../)
* namespace [Aspose.Zip.Wim](../../wimloadoptions/)
* assembly [Aspose.Zip](../../../)


