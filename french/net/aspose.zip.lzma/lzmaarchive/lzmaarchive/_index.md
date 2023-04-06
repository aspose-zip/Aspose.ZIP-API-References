---
title: LzmaArchive.LzmaArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: LzmaArchive constructeur. Initialise une nouvelle instance duLzmaArchive classe et compose larchive au format lzma.
type: docs
weight: 10
url: /fr/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Initialise une nouvelle instance du[`LzmaArchive`](../) classe et compose l'archive au format lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Ensemble de paramètres d'archive lzma particulière. |

### Voir également

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* espace de noms [Aspose.Zip.LZMA](../../lzmaarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Initialise une nouvelle instance du[`LzmaArchive`](../) classe préparée pour la décompression.

```csharp
public LzmaArchive(Stream source)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| source | Stream | La source des archives. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *source* n'est pas recherchable. |
| ArgumentNullException | *source* est nul. |

### Remarques

Ce constructeur ne se décompresse pas. Voir[`Extract`](../extract/) méthode de décompression.

### Voir également

* class [LzmaArchive](../)
* espace de noms [Aspose.Zip.LZMA](../../lzmaarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Initialise une nouvelle instance du[`LzmaArchive`](../) classe préparée pour la décompression.

```csharp
public LzmaArchive(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès à la source de l'archive. |

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

Ce constructeur ne se décompresse pas. Voir[`Extract`](../extract/) méthode de décompression.

### Exemples

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Voir également

* class [LzmaArchive](../)
* espace de noms [Aspose.Zip.LZMA](../../lzmaarchive/)
* Assemblée [Aspose.Zip](../../../)


