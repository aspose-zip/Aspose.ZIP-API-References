---
title: SevenZipArchiveEntry.Extract
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipArchiveEntry méthode. Extrait lentrée du système de fichiers par le chemin fourni.
type: docs
weight: 80
url: /fr/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

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
| ArgumentException | Le*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
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

* class [SevenZipArchiveEntry](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Assemblée [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extrait l'entrée du flux fourni.

```csharp
public void Extract(Stream destination, string password = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être inscriptible. |
| password | String | Mot de passe facultatif pour le déchiffrement. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |
| InvalidOperationException | L'archive n'est pas ouverte pour l'extraction. - ou - Cette entrée est un répertoire. |
| InvalidDataException | Données erronées dans l'entrée. |

### Exemples

Extraire une entrée d'archive zip avec mot de passe.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Voir également

* class [SevenZipArchiveEntry](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Assemblée [Aspose.Zip](../../../)


