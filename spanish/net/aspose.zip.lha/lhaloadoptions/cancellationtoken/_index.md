---
title: "LhaLoadOptions.CancellationToken"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad LhaLoadOptions. Obtiene o establece un token de cancelación usado para cancelar la operación de extracción."
type: docs
weight: 20
url: /es/net/aspose.zip.lha/lhaloadoptions/cancellationtoken/
---
## LhaLoadOptions.CancellationToken property

Obtiene o establece un token de cancelación utilizado para cancelar la operación de extracción.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Observaciones

Esta propiedad existe para .NET Framework 4.0 y superiores.

## Ejemplos

Cancelar la extracción del archivo LHA después de un tiempo determinado.

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

Uso con `Task`

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

La cancelación generalmente resulta en que algunos datos no se extraigan.

### Ver también

* class [LhaLoadOptions](../)
* namespace [Aspose.Zip.Lha](../../lhaloadoptions/)
* assembly [Aspose.Zip](../../../)


