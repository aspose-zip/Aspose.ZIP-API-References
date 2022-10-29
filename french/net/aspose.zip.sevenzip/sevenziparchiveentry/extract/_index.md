---
title: Extract
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Extrait lentrée du système de fichiers par le chemin fourni.
type: docs
weight: 60
url: /fr/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## SevenZipArchiveEntry.Extract method

Extrait l'entrée du système de fichiers par le chemin fourni.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier de destination. Si le fichier existe déjà, il sera écrasé. |
| password | String | Mot de passe facultatif pour le déchiffrement. |

### Return_Value

Les informations de fichier du fichier composé.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | La*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Exemples

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Voir également

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchiveentry)
* Assemblée [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->