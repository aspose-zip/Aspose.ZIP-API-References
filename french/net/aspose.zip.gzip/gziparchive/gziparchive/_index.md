---
title: GzipArchive.GzipArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: GzipArchive constructeur. Initialise une nouvelle instance duGzipArchive classe préparée pour la compression.
type: docs
weight: 10
url: /fr/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Initialise une nouvelle instance du[`GzipArchive`](../) classe préparée pour la compression.

```csharp
public GzipArchive()
```

### Exemples

L'exemple suivant montre comment compresser un fichier.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Voir également

* class [GzipArchive](../)
* espace de noms [Aspose.Zip.Gzip](../../gziparchive/)
* Assemblée [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Initialise une nouvelle instance du[`GzipArchive`](../) classe préparée pour la décompression.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceStream | Stream | La source des archives. |
| parseHeader | Boolean | Indique s'il faut analyser l'en-tête du flux pour déterminer les propriétés, y compris le nom. N'a de sens que pour le flux de recherche. |

### Remarques

Ce constructeur ne se décompresse pas. Voir[`Open`](../open/) méthode de décompression.

### Exemples

Ouvrez une archive à partir d'un flux et extrayez-la dans un`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Voir également

* class [GzipArchive](../)
* espace de noms [Aspose.Zip.Gzip](../../gziparchive/)
* Assemblée [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Initialise une nouvelle instance du[`GzipArchive`](../) classe.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier d'archive. |
| parseHeader | Boolean | Indique s'il faut analyser l'en-tête du flux pour déterminer les propriétés, y compris le nom. N'a de sens que pour le flux de recherche. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Ce constructeur ne se décompresse pas. Voir[`Open`](../open/) méthode de décompression.

### Exemples

Ouvrez une archive à partir d'un fichier par chemin et extrayez-la dans un`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Voir également

* class [GzipArchive](../)
* espace de noms [Aspose.Zip.Gzip](../../gziparchive/)
* Assemblée [Aspose.Zip](../../../)


