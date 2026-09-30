---
title: "CabLoadOptions.CancellationToken"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà CabLoadOptions. Ottiene o imposta un token di cancellazione utilizzato per annullare l'operazione di estrazione"
type: docs
weight: 20
url: /it/net/aspose.zip.cab/cabloadoptions/cancellationtoken/
---
## CabLoadOptions.CancellationToken property

Ottiene o imposta un token di cancellazione utilizzato per annullare l'operazione di estrazione.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Osservazioni

Questa proprietà esiste per .NET Framework 4.0 e versioni successive.

## Esempi

Annulla l'estrazione dell'archivio CAB dopo un certo periodo di tempo.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new CabArchive("big.cab", new CabLoadOptions() { CancellationToken = cts.Token }))
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

Utilizzo con `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new CabLoadOptions() { CancellationToken = cts.Token };
    using (var a = new CabArchive("big.cab", loadOptions))
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

* class [CabLoadOptions](../)
* namespace [Aspose.Zip.Cab](../../cabloadoptions/)
* assembly [Aspose.Zip](../../../)


