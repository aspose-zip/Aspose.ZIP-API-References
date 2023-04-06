---
title: XzArchive.Extract
second_title: Référence de l'API Aspose.ZIP pour .NET
description: XzArchive méthode. Extrait larchive xz dans un flux.
type: docs
weight: 30
url: /fr/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

Extrait l'archive xz dans un flux.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destination | Stream | Flux pour stocker des données décompressées. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Les en-têtes d'archive et les informations de service n'ont pas été lus. |

### Exemples

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Voir également

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrait l'archive xz dans un fichier.

```csharp
public void Extract(FileInfo fileInfo)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo pour stocker les données décompressées. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Les en-têtes d'archive et les informations de service n'ont pas été lus. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour ouvrir le*fileInfo*. |
| ArgumentException | Le chemin du fichier est vide ou ne contient que des espaces blancs. |
| FileNotFoundException | Le fichier est introuvable. |
| UnauthorizedAccessException | Le chemin d'accès au fichier est en lecture seule ou est un répertoire. |
| ArgumentNullException | *fileInfo* est nul. |
| DirectoryNotFoundException | Le chemin spécifié n'est pas valide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |

### Exemples

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Voir également

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrait l'archive xz dans un fichier par chemin.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier qui stockera les données décompressées. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Les en-têtes d'archive et les informations de service n'ont pas été lus. |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Exemples

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Voir également

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)


