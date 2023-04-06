---
title: Archive.SaveSplit
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Archive méthode. Enregistre larchive multivolume dans le répertoire de destination fourni.
type: docs
weight: 100
url: /fr/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Enregistre l'archive multi-volume dans le répertoire de destination fourni.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationDirectory | String | Chemin d'accès au répertoire dans lequel les segments d'archive doivent être créés. |
| options | SplitArchiveSaveOptions | Options d'enregistrement d'archives, y compris le nom de fichier. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Cette archive a été ouverte à partir d'une source existante. |
| NotSupportedException | Cette archive est à la fois compressée avec la méthode XZ et cryptée. |
| ArgumentNullException | *destinationDirectory* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder au répertoire. |
| ArgumentException | *destinationDirectory* contient des caractères non valides tels que ", &gt;, &lt; ou &#x7C;. |
| PathTooLongException | Le chemin spécifié dépasse la longueur maximale définie par le système. |

### Remarques

Cette méthode compose plusieurs (`n`) fichiers nomfichier.z01, nomfichier.z02, ..., nomfichier.z(n-1), nomfichier.zip.

Impossible de rendre l'archive existante multi-volume.

### Exemples

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Voir également

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* espace de noms [Aspose.Zip](../../archive/)
* Assemblée [Aspose.Zip](../../../)


