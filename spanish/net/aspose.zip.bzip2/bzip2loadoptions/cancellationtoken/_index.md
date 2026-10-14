---
title: "Bzip2LoadOptions.CancellationToken"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad de Bzip2LoadOptions. Obtiene o establece un token de cancelación usado para cancelar la operación de extracción"
type: docs
weight: 20
url: /es/net/aspose.zip.bzip2/bzip2loadoptions/cancellationtoken/
---
## Bzip2LoadOptions.CancellationToken property

Obtiene o establece un token de cancelación utilizado para cancelar la operación de extracción.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Observaciones

Esta propiedad existe para .NET Framework 4.0 y superiores.

## Ejemplos

Cancelar la extracción del archivo Bzip2 después de un tiempo determinado.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new Bzip2Archive("big.bz2", new Bzip2LoadOptions() { CancellationToken = cts.Token }))
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

Uso con `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new Bzip2LoadOptions() { CancellationToken = cts.Token };
    using (var a = Bzip2Archive("big.bz2", loadOptions))
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

* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


