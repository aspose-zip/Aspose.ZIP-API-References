---
title: "LzxLoadOptions.CancellationToken"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà LzxLoadOptions. Ottiene o imposta un token di cancellazione usato per annullare l'operazione di estrazione"
type: docs
weight: 20
url: /it/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Ottiene o imposta un token di cancellazione utilizzato per annullare l'operazione di estrazione.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Osservazioni

Questa proprietà esiste per .NET Framework 4.0 e versioni successive.

## Esempi

Annulla l'estrazione dell'archivio Lzx dopo un certo tempo.

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

Utilizzo con `Task`

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

La cancellazione di solito comporta che alcuni dati non vengano estratti.

### Vedi anche

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


