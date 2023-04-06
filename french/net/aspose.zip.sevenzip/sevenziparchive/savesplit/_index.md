---
title: SevenZipArchive.SaveSplit
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipArchive méthode. Enregistre larchive multivolume dans le répertoire de destination fourni.
type: docs
weight: 90
url: /fr/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Enregistre l'archive multi-volume dans le répertoire de destination fourni.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationDirectory | String | Chemin d'accès au répertoire dans lequel les segments d'archive doivent être créés. |
| options | SplitSevenZipArchiveSaveOptions | Options d'enregistrement d'archives, y compris le nom de fichier. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Cette archive a été ouverte à partir d'une source existante. |
| ArgumentNullException | *destinationDirectory* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder au répertoire. |
| ArgumentException | *destinationDirectory* contient des caractères non valides tels que ", &gt;, &lt; ou &#x7C;. |
| PathTooLongException | Le chemin spécifié dépasse la longueur maximale définie par le système. |

### Remarques

Cette méthode compose plusieurs (`n`) fichiers nomfichier.7z.001, nomfichier.7z.002, ..., nomfichier.7z.(n).

Impossible de rendre l'archive existante multi-volume.

### Exemples

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Voir également

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Assemblée [Aspose.Zip](../../../)


