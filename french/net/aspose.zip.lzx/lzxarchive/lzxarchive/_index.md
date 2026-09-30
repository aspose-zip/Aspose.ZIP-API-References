---
title: "LzxArchive.LzxArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur LzxArchive. Initialise une nouvelle instance de la classe LzxArchive et compose une liste d'entrées pouvant être extraites de l'archive"
type: docs
weight: 10
url: /fr/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Initialise une nouvelle instance de la classe [`LzxArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| extractionSource | Stream | La source de l'archive. |
| loadOptions | LzxLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *extractionSource* est nul. |
| ArgumentException | *extractionSource* ne prend pas en charge la recherche. |
| InvalidDataException | Signature incorrecte pour l'archive. - ou - Le fichier n'est pas une archive LZX. |
| NotImplementedException | L'archive Lzx contient des entrées fusionnées. |
| EndOfStreamException | Le flux *extractionSource* est trop court. |
| ObjectDisposedException | Lancé si le flux a été fermé. |
| IOException | Une erreur d'E/S se produit. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir la méthode [`Extract`](../../lzxarchiveentry/extract/) pour la décompression.

### Voir aussi

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`LzxArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin complet ou relatif vers le fichier d'archive. |
| loadOptions | LzxLoadOptions | Options pour charger une archive existante. |

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
| InvalidDataException | Le fichier est corrompu. |
| NotImplementedException | L'archive Lzx contient des entrées fusionnées. |
| EndOfStreamException | Le fichier est trop court. |
| ObjectDisposedException | Lancé si le flux a été fermé. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir la méthode [`Extract`](../../lzxarchiveentry/extract/) pour la décompression.

## Exemples

L'exemple suivant extrait une archive, puis décompresse la première entrée dans un `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Voir aussi

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


