---
title: "XarArchive.CreateEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode XarArchive. Crée une entrée unique dans l'archive"
type: docs
weight: 40
url: /fr/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Crée une seule entrée dans l'archive.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| fileInfo | FileInfo | Les métadonnées du fichier ou du dossier à compresser. |
| openImmediately | Boolean | True, si le fichier doit être ouvert immédiatement, sinon le fichier sera ouvert lors de l'enregistrement de l'archive. |
| compressionSettings | XarCompressionSettings | Les paramètres de compression utilisés pour l'élément [`XarEntry`](../../xarentry/) ajouté. |

### Valeur de retour

Instance d'entrée Xar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* est nul. |
| ArgumentException | *name* est vide. |
| ArgumentNullException | *fileInfo* est nul. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

Si le fichier est ouvert immédiatement avec le paramètre *openImmediately*, il devient bloqué jusqu'à ce que l'archive soit libérée.

## Exemples

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Voir aussi

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Crée une seule entrée dans l'archive.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| sourcePath | String | Chemin du fichier à compresser. |
| openImmediately | Boolean | True, si le fichier doit être ouvert immédiatement, sinon le fichier sera ouvert lors de l'enregistrement de l'archive. |
| compressionSettings | XarCompressionSettings | Les paramètres de compression utilisés pour l'élément [`XarEntry`](../../xarentry/) ajouté. |

### Valeur de retour

Instance d'entrée Xar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourcePath* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *sourcePath* est vide, ne contient que des espaces blancs, ou contient des caractères invalides. - ou - Le nom de fichier, en tant que partie de *name*, dépasse 100 symboles. |
| UnauthorizedAccessException | L'accès au fichier *sourcePath* est refusé. |
| PathTooLongException | Le *sourcePath* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères, et les noms de fichier moins de 260 caractères. - ou - *name* est trop long pour xar. |
| NotSupportedException | Le fichier à *sourcePath* contient deux‑points (:) au milieu de la chaîne. |
| InvalidOperationException | Impossible de modifier l'archive xar. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

Le nom de l'entrée est uniquement défini dans le paramètre *name*. Le nom de fichier fourni dans le paramètre *sourcePath* n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec le paramètre *openImmediately*, il devient bloqué jusqu'à ce que l'archive soit libérée.

## Exemples

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Voir aussi

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Crée une seule entrée dans l'archive.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |
| compressionSettings | XarCompressionSettings | Les paramètres de compression utilisés pour l'élément [`XarEntry`](../../xarentry/) ajouté. |

### Valeur de retour

Instance d'entrée Xar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* est nul. |
| ArgumentNullException | *source* est nul. |
| ArgumentException | *name* est vide. |
| InvalidOperationException | Impossible de modifier l'archive xar. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Voir aussi

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


