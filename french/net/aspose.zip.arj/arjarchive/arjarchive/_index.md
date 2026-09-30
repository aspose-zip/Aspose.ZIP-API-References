---
title: "ArjArchive.ArjArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur ArjArchive. Initialise une nouvelle instance de la classe ArjArchive et compose une liste d'entrées pouvant être extraites de l'archive."
type: docs
weight: 10
url: /fr/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Initialise une nouvelle instance de la classe [`ArjArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| extractionSource | Stream | La source de l'archive. |
| loadOptions | ArjLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *extractionSource* est nul. |
| ArgumentException | &gt;*extractionSource* ne prend pas en charge la recherche. |
| InvalidDataException | Signature incorrecte pour l'archive. - ou - Le fichier n'est pas une archive ARJ. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte avant que tous les octets d’en‑tête ou de nom aient été lus. |
| NotSupportedException | L’archive est corrompue. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir la méthode [`Extract`](../../arjentryplain/extract/) pour la décompression.

### Voir aussi

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`ArjArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin vers le fichier d'archive. |
| loadOptions | ArjLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| FileNotFoundException | Le fichier est introuvable. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte avant que tous les octets d’en‑tête ou de nom aient été lus. |
| InvalidDataException | Le nombre magique ARJ est invalide ou la taille de l’en‑tête est hors limites. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir la méthode [`Extract`](../../arjentryplain/extract/) pour la décompression.

## Exemples

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Voir aussi

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


