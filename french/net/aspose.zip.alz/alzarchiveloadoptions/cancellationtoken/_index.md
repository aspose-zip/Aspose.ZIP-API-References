---
title: "AlzArchiveLoadOptions.CancellationToken"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété AlzArchiveLoadOptions. Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction"
type: docs
weight: 20
url: /fr/net/aspose.zip.alz/alzarchiveloadoptions/cancellationtoken/
---
## AlzArchiveLoadOptions.CancellationToken property

Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarques

Cette propriété existe pour .NET Framework 4.0 et supérieur.

## Exemples

Annuler l'extraction de l'archive ALZ après un certain temps.

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

### Voir aussi

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


