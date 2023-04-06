---
title: XzArchive.XzArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: XzArchive constructeur. Initialise une nouvelle instance duXzArchive classe et compose larchive au format xz.
type: docs
weight: 10
url: /fr/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Initialise une nouvelle instance du[`XzArchive`](../) classe et compose l'archive au format xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| settings | XzArchiveSettings | Ensemble de paramètres d'archive xz particuliers : taille du dictionnaire, taille du bloc, type de contrôle. |

### Voir également

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Initialise une nouvelle instance du[`XzArchive`](../) classe préparée pour la décompression.

```csharp
public XzArchive(Stream source)
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

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Initialise une nouvelle instance du[`XzArchive`](../) classe préparée pour la décompression.

```csharp
public XzArchive(string path)
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

### Voir également

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)


