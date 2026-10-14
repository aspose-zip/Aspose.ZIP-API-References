---
title: "AlzArchiveLoadOptions.CancellationToken"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "AlzArchiveLoadOptions property. Obtiene o establece un token de cancelación usado para cancelar la operación de extracción"
type: docs
weight: 20
url: /es/net/aspose.zip.alz/alzarchiveloadoptions/cancellationtoken/
---
## AlzArchiveLoadOptions.CancellationToken property

Obtiene o establece un token de cancelación utilizado para cancelar la operación de extracción.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Observaciones

Esta propiedad existe para .NET Framework 4.0 y superiores.

## Ejemplos

Cancelar la extracción del archivo ALZ después de un tiempo determinado.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new AlzArchive("big.alz", new AlzArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
            archive.Entries[0].Extract("data.bin");
        }
        catch(OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

### Ver también

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


