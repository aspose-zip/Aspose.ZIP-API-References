---
title: ArchiveLoadOptions.EntryListed
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveLoadOptions propriété. Obtient ou définit le délégué appelé lorsquune entrée est répertoriée dans la table des matières.
type: docs
weight: 50
url: /fr/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Obtient ou définit le délégué appelé lorsqu'une entrée est répertoriée dans la table des matières.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Exemples

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Voir également

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* espace de noms [Aspose.Zip](../../archiveloadoptions/)
* Assemblée [Aspose.Zip](../../../)


