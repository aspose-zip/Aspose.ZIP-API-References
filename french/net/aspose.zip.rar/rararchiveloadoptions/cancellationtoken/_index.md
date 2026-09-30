---
title: "RarArchiveLoadOptions.CancellationToken"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété RarArchiveLoadOptions. Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction"
type: docs
weight: 20
url: /fr/net/aspose.zip.rar/rararchiveloadoptions/cancellationtoken/
---
## RarArchiveLoadOptions.CancellationToken property

Obtient ou définit un jeton d'annulation utilisé pour annuler l'opération d'extraction.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Remarques

Cette propriété existe pour .NET Framework 4.0 et supérieur.

## Exemples

Annuler l'extraction de l'archive RAR après un certain temps.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new RarArchive("big.rar", new RarArchiveLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new RarArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new RarArchive("big.rar", loadOptions))
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

* class [RarArchiveLoadOptions](../)
* namespace [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


