---
title: "XarArchive.DeleteEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode XarArchive. Supprime la première occurrence d'une entrée spécifique de la liste d'entrées"
type: docs
weight: 50
url: /fr/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Supprime la première occurrence d'une entrée spécifique de la liste d'entrées.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| entrée | XarEntry | L'entrée à supprimer de la liste d'entrées. |

### Valeur de retour

Instance d'entrée Xar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *entry* est nul. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | L'archive n'est pas ouverte pour l'extraction. |

## Exemples

Voici comment vous pouvez supprimer toutes les entrées sauf la dernière :

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Voir aussi

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


