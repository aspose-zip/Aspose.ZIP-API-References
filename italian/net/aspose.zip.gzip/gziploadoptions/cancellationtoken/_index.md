---
title: "GzipLoadOptions.CancellationToken"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà GzipLoadOptions. Ottiene o imposta un token di cancellazione usato per annullare l'operazione di estrazione."
type: docs
weight: 20
url: /it/net/aspose.zip.gzip/gziploadoptions/cancellationtoken/
---
## GzipLoadOptions.CancellationToken property

Ottiene o imposta un token di cancellazione utilizzato per annullare l'operazione di estrazione.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Osservazioni

Questa proprietà esiste per .NET Framework 4.0 e versioni successive.

## Esempi

Annulla l'estrazione dell'archivio gzip dopo un certo periodo.

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

Utilizzo con `Task`

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

La cancellazione di solito comporta che alcuni dati non vengano estratti.

### Vedi anche

* class [GzipLoadOptions](../)
* namespace [Aspose.Zip.Gzip](../../gziploadoptions/)
* assembly [Aspose.Zip](../../../)


