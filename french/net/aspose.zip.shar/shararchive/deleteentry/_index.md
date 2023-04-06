---
title: SharArchive.DeleteEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SharArchive méthode. Supprime la première occurrence dune entrée spécifique de la liste des entrées.
type: docs
weight: 50
url: /fr/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Supprime la première occurrence d'une entrée spécifique de la liste des entrées.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| entry | SharEntry | Entrée à supprimer de la liste des entrées. |

### Return_Value

Instance d'entrée Shar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *entry* est nul. |

### Exemples

Voici comment vous pouvez supprimer toutes les entrées sauf la dernière :

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Voir également

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Supprime l'entrée de la liste des entrées par index.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| entryIndex | Int32 | Index de base zéro de l'entrée à supprimer. |

### Return_Value

L'archive avec l'entrée supprimée.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* est inférieur à 0.-ou-*entryIndex* est égal ou supérieur à`Entrées` compter. |

### Exemples

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Voir également

* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)


