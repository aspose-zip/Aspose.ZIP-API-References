---
title: "EggArchiveLoadOptions.CancellationToken"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété EggArchiveLoadOptions. Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction"
type: docs
weight: 20
url: /fr/net/aspose.zip.egg/eggarchiveloadoptions/cancellationtoken/
---
## EggArchiveLoadOptions.CancellationToken property

Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarques

Cette propriété existe pour .NET Framework 4.0 et supérieur.

## Exemples

Annuler l'extraction de l'archive EGG après un certain temps.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new EggArchive("big.egg", new EggArchiveLoadOptions() { CancellationToken = cts.Token }))
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

* class [EggArchiveLoadOptions](../)
* namespace [Aspose.Zip.Egg](../../eggarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


