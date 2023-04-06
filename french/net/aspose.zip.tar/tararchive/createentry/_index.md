---
title: TarArchive.CreateEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Créer une entrée unique dans larchive.
type: docs
weight: 80
url: /fr/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Créer une entrée unique dans l'archive.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |
| fileInfo | FileSystemInfo | Les métadonnées du fichier ou du dossier à compresser. |

### Return_Value

Instance d'entrée tar.

### Exceptions

| exception | condition |
| --- | --- |
| PathTooLongException | *name* est trop long pour tar selon la norme IEEE 1003.1-1998. |
| ArgumentException | Nom de fichier, dans le cadre de*name*, dépasse 100 symboles. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*fileInfo* Le paramètre n'affecte pas le nom de l'entrée.

*fileInfo* peut faire référence àDirectoryInfo si l'entrée est répertoire.

### Exemples

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Voir également

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Créer une entrée unique dans l'archive.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| fileInfo | FileInfo | Les métadonnées du fichier ou du dossier à compresser. |
| openImmediately | Boolean | Vrai si ouvrir le fichier immédiatement, sinon ouvrir le fichier lors de l'enregistrement de l'archive. |

### Return_Value

Instance d'entrée tar.

### Exceptions

| exception | condition |
| --- | --- |
| PathTooLongException | *name* est trop long pour tar selon la norme IEEE 1003.1-1998. |
| ArgumentException | Nom de fichier, dans le cadre de*name*, dépasse 100 symboles. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*fileInfo* Le paramètre n'affecte pas le nom de l'entrée.

*fileInfo* peut faire référence àDirectoryInfo si l'entrée est répertoire.

Si le fichier est ouvert immédiatement avec*openImmediately*paramètre, il devient bloqué jusqu'à ce que l'archive soit supprimée.

### Exemples

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Voir également

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Créer une entrée unique dans l'archive.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| path | String | Chemin d'accès au fichier à compresser. |
| openImmediately | Boolean | Vrai si ouvrir le fichier immédiatement, sinon ouvrir le fichier lors de l'enregistrement de l'archive. |

### Return_Value

Instance d'entrée tar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. - ou - Nom de fichier, dans le cadre de*name*, dépasse 100 symboles. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path* , nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. - ou -*name* est trop long pour tar selon la norme IEEE 1003.1-1998. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*path* Le paramètre n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec*openImmediately*paramètre, il devient bloqué jusqu'à ce que l'archive soit supprimée.

### Exemples

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Voir également

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


