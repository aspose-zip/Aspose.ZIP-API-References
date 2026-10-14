---
title: "AppleArchive.CreateEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode AppleArchive. Crée une seule entrée dans l'archive"
type: docs
weight: 60
url: /fr/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Crée une entrée unique dans l'archive.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| chemin | String | Le chemin du fichier à compresser. |
| openImmediately | Boolean | True, si le fichier doit être ouvert immédiatement, sinon le fichier sera ouvert lors de l'enregistrement de l'archive. |

### Valeur de retour

Instance d'entrée Apple Archive.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée. |
| ArgumentException | *name* est vide. |
| ArgumentNullException | *path* est `null`. |

### Voir aussi

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Crée une entrée unique dans l'archive.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |

### Valeur de retour

Instance d'entrée Apple Archive.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée. |
| ArgumentException | *name* est vide. |
| ArgumentNullException | *source* est `null`. |

### Voir aussi

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Crée une entrée unique dans l'archive.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| fileInfo | FileInfo | Les métadonnées du fichier à compresser. |
| openImmediately | Boolean | True, si le fichier doit être ouvert immédiatement, sinon le fichier sera ouvert lors de l'enregistrement de l'archive. |

### Valeur de retour

Instance d'entrée Apple Archive.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée. |
| ArgumentException | *name* est vide. |
| ArgumentNullException | *fileInfo* est `null`. |

### Voir aussi

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


