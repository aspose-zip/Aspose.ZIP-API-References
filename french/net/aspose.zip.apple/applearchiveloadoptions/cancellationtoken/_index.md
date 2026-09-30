---
title: "AppleArchiveLoadOptions.CancellationToken"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété AppleArchiveLoadOptions. Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction"
type: docs
weight: 20
url: /fr/net/aspose.zip.apple/applearchiveloadoptions/cancellationtoken/
---
## AppleArchiveLoadOptions.CancellationToken property

Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarques

Cette propriété existe pour .NET Framework 4.0 et supérieur.

## Exemples

Annuler l'extraction Apple Archive après un certain temps.

```csharp
using (System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource())
{
    cts.CancelAfter(System.TimeSpan.FromSeconds(60)); 
    using (var a = new AppleArchive("big.aar", new AppleArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.ExtractToDirectory("destination");
        }
        catch(System.OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

Utilisation avec `Task`

```csharp
System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource();
cts.CancelAfter(System.TimeSpan.FromSeconds(60));
System.Threading.Tasks.Task t = System.Threading.Tasks.Task.Run(delegate()
{
    var loadOptions = new AppleArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new AppleArchive("big.aar", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(System.Threading.Tasks.Task antecedent)
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

* class [AppleArchiveLoadOptions](../)
* namespace [Aspose.Zip.Apple](../../applearchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


