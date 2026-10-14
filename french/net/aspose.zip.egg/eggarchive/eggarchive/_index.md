---
title: "EggArchive.EggArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur EggArchive. Initialise une nouvelle instance de la classe EggArchive à partir d'un flux"
type: docs
weight: 10
url: /fr/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Initialise une nouvelle instance de la classe [`EggArchive`](../) à partir d'un flux.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux d'archive EGG. Le flux doit prendre en charge la lecture et le positionnement. |
| loadOptions | EggArchiveLoadOptions | Options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* est nul. |
| ArgumentException | *stream* n'est pas lisible et recherchable. |

### Voir aussi

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`EggArchive`](../) à partir d'un chemin de fichier.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Chemin du fichier d'archive EGG. |
| loadOptions | EggArchiveLoadOptions | Options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| FileNotFoundException | Le fichier n'existe pas. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| FileNotFoundException | Le fichier est introuvable. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |

### Voir aussi

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


