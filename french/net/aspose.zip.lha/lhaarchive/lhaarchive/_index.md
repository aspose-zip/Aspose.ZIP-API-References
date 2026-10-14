---
title: "LhaArchive.LhaArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur LhaArchive. Initialise une nouvelle instance de la classe LhaArchive et compose une liste d'entrées pouvant être extraites de l'archive."
type: docs
weight: 10
url: /fr/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Initialise une nouvelle instance de la classe [`LhaArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | La source de l'archive. |
| loadOptions | LhaLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* est nul |
| ArgumentException | *sourceStream* n'est pas séekable. |
| InvalidDataException | Données inappropriées trouvées. |
| EndOfStreamException | Lancé lorsque la fin du flux est atteinte avant que le nombre attendu d'octets ne soit lu. |
| ObjectDisposedException | Lancé lorsque l'objet a été libéré. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir la méthode [`Extract`](../../lhaarchiveentry/extract/) pour la décompression.

### Voir aussi

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`LhaArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin complet ou relatif vers le fichier d'archive. |
| loadOptions | LhaLoadOptions | Options pour charger une archive existante. |

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
| EndOfStreamException | Lancé lorsque la fin du flux est atteinte avant que le nombre attendu d'octets ne soit lu. |
| ObjectDisposedException | Lancé lorsque l'objet a été libéré. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir la méthode [`Extract`](../../lhaarchiveentry/extract/) pour la décompression.

## Exemples

L'exemple suivant extrait une archive, puis décompresse la première entrée dans un `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Voir aussi

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


