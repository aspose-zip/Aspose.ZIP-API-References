---
title: "ArchiveFactory.CompressDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode ArchiveFactory. Compresse le répertoire spécifié dans un fichier d’archive en utilisant le format d’archive fourni"
type: docs
weight: 10
url: /fr/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Compresse le répertoire spécifié dans un fichier d’archive en utilisant le format d’archive fourni.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du répertoire qui sera compressé. |
| outputFileName | String | Nom du fichier de destination. |
| archiveFormat | ArchiveFormat | Le format de l’archive à créer (par ex., zip, rar, tar, etc.). |

### Exceptions

| exception | condition |
| --- | --- |
| DirectoryNotFoundException | Lancée si le répertoire spécifié par *path* n’existe pas. |
| ArgumentException | Lancée si *path* est nul ou une chaîne vide. |
| NotSupportedException | Lancée si le *archiveFormat* spécifié n’est pas pris en charge ou reconnu. |
| ArgumentNullException | *path* est `null`. |

## Remarques

Cette méthode créera un fichier d’archive à l’emplacement spécifié par le paramètre *path*. Le nom du fichier d’archive sera généralement le nom du répertoire suivi de l’extension de fichier appropriée en fonction du *archiveFormat*. Le répertoire lui‑même n’est pas modifié ni supprimé.

## Exemples

Voici un exemple d'utilisation de la méthode CompressDirectory :

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Cela créera un fichier ZIP avec le contenu du répertoire au chemin spécifié.
```

### Voir aussi

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


