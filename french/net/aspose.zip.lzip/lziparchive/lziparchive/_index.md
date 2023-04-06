---
title: LzipArchive.LzipArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: LzipArchive constructeur. Initialise une nouvelle instance duLzipArchive .
type: docs
weight: 10
url: /fr/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Initialise une nouvelle instance du[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| settings | LzipArchiveSettings | Paramétrage d'une archive lzip particulière avec définition de la taille du dictionnaire. |

### Voir également

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* espace de noms [Aspose.Zip.Lzip](../../lziparchive/)
* Assemblée [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Initialise une nouvelle instance du[`LzipArchive`](../) classe préparée pour la décompression.

```csharp
public LzipArchive(Stream sourceStream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceStream | Stream | La source des archives. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *sourceStream* n'est pas recherchable. |
| ArgumentNullException | *sourceStream* est nul. |
| InvalidDataException | Les en-têtes ne correspondent pas au type d'archive lzip. |

### Remarques

Ce constructeur ne se décompresse pas. Voir[`Extract`](../extract/) méthode de décompression.

### Voir également

* class [LzipArchive](../)
* espace de noms [Aspose.Zip.Lzip](../../lziparchive/)
* Assemblée [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Initialise une nouvelle instance du[`LzipArchive`](../) classe préparée pour la décompression.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | Les en-têtes ne correspondent pas au type d'archive lzip. |

### Remarques

Ce constructeur ne se décompresse pas. Voir[`Extract`](../extract/) méthode de décompression.

### Exemples

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Voir également

* class [LzipArchive](../)
* espace de noms [Aspose.Zip.Lzip](../../lziparchive/)
* Assemblée [Aspose.Zip](../../../)


