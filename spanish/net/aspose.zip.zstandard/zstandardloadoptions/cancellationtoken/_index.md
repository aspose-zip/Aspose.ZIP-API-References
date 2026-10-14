---
title: "ZstandardLoadOptions.CancellationToken"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad ZstandardLoadOptions. Obtiene o establece un token de cancelación utilizado para cancelar la operación de extracción."
type: docs
weight: 20
url: /es/net/aspose.zip.zstandard/zstandardloadoptions/cancellationtoken/
---
## ZstandardLoadOptions.CancellationToken property

Obtiene o establece un token de cancelación utilizado para cancelar la operación de extracción.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Observaciones

Esta propiedad existe para .NET Framework 4.0 y superiores.

## Ejemplos

Cancelar la extracción del archivo Zstandard después de un tiempo determinado.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new ZstandardArchive("big.zstd", new ZStandardLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new ZStandardLoadOptions() { CancellationToken = cts.Token };
    using (var a = ZstandardArchive("big.zstd", loadOptions))
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

* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


