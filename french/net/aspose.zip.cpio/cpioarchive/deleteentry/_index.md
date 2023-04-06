---
title: CpioArchive.DeleteEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: CpioArchive méthode. Supprime la première occurrence dune entrée spécifique de la liste des entrées.
type: docs
weight: 50
url: /fr/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Supprime la première occurrence d'une entrée spécifique de la liste des entrées.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| entry | CpioEntry | Entrée à supprimer de la liste des entrées. |

### Return_Value

Instance d'entrée Cpio.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *entry* est nul. |

### Exemples

Voici comment vous pouvez supprimer toutes les entrées sauf la dernière :

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Voir également

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Supprime l'entrée de la liste des entrées par index.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Voir également

* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)


