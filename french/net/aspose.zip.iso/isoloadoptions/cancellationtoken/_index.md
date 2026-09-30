---
title: "IsoLoadOptions.CancellationToken"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété IsoLoadOptions. Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction"
type: docs
weight: 20
url: /fr/net/aspose.zip.iso/isoloadoptions/cancellationtoken/
---
## IsoLoadOptions.CancellationToken property

Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarques

Cette propriété existe pour .NET Framework 4.0 et supérieur.

## Exemples

Annuler l'extraction de l'archive ISO après un certain temps.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new IsoArchive("big.iso", new IsoLoadOptions() { CancellationToken = cts.Token }))
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

Utilisation avec `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new ArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = Archive("big.iso", loadOptions))
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

L'annulation entraîne généralement que certaines données ne soient pas extraites.

### Voir aussi

* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


