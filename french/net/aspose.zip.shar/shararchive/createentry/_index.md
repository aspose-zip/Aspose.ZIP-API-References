---
title: SharArchive.CreateEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SharArchive méthode. Créer une entrée unique dans larchive.
type: docs
weight: 40
url: /fr/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Créer une entrée unique dans l'archive.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| fileInfo | FileInfo | Les métadonnées du fichier ou du dossier à compresser. |
| openImmediately | Boolean | Vrai si ouvrir le fichier immédiatement, sinon ouvrir le fichier lors de l'enregistrement de l'archive. |

### Return_Value

Instance d'entrée Shar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* est nul. |
| ArgumentException | *name* est vide. |
| ArgumentNullException | *fileInfo* est nul. |

### Remarques

Si le fichier est ouvert immédiatement avec*openImmediately*paramètre, il devient bloqué jusqu'à ce que l'archive soit supprimée.

### Exemples

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Voir également

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Créer une entrée unique dans l'archive.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| sourcePath | String | Chemin d'accès au fichier à compresser. |
| openImmediately | Boolean | Vrai si ouvrir le fichier immédiatement, sinon ouvrir le fichier lors de l'enregistrement de l'archive. |

### Return_Value

Instance d'entrée Shar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourcePath* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*sourcePath* est vide, ne contient que des espaces blancs ou contient des caractères non valides. - ou - Nom de fichier, dans le cadre de*name*, dépasse 100 symboles. |
| UnauthorizedAccessException | Accéder au dossier*sourcePath* est refusé. |
| PathTooLongException | Le spécifié*sourcePath* , nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. - ou -*name* est trop long pour shar. |
| NotSupportedException | Fichier à*sourcePath* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*sourcePath* Le paramètre n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec*openImmediately*paramètre, il devient bloqué jusqu'à ce que l'archive soit supprimée.

### Exemples

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Voir également

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Créer une entrée unique dans l'archive.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |

### Return_Value

Instance d'entrée Shar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* est nul. |
| ArgumentNullException | *source* est nul. |
| ArgumentException | *name* est vide. |

### Exemples

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Voir également

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)


