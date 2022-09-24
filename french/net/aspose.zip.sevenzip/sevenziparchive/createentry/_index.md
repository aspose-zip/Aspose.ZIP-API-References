---
title: CreateEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Créer une entrée unique dans larchive.
type: docs
weight: 50
url: /fr/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Créer une entrée unique dans l'archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| fileInfo | FileInfo | Les métadonnées du fichier à compresser. |
| openImmediately | Boolean | Vrai si ouvrir le fichier immédiatement, sinon ouvrir le fichier lors de l'enregistrement de l'archive. |
| newEntrySettings | SevenZipEntrySettings | Paramètres de compression et de cryptage utilisés pour les[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Objet. |

### Return_Value

Instance d'entrée Seven Zip.

### Exceptions

| exception | condition |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* est en lecture seule ou est un répertoire. |
| DirectoryNotFoundException | Le chemin spécifié n'est pas valide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*fileInfo* Le paramètre n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec*openImmediately* paramètre, il devient bloqué jusqu'à ce que l'archive soit enregistrée.

### Exemples

Composez une archive avec des entrées cryptées avec des mots de passe différents chacune.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Voir également

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Créer une entrée unique dans l'archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |
| newEntrySettings | SevenZipEntrySettings | Paramètres de compression et de cryptage utilisés pour les[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Objet. |
| fileInfo | FileSystemInfo | Les métadonnées du fichier ou du dossier à compresser. |

### Return_Value

Instance d'entrée SevenZip.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Tous les deux*source* et*fileInfo* sont nuls ou*source* est nul et*fileInfo* signifie répertoire. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*fileInfo* Le paramètre n'affecte pas le nom de l'entrée.

*fileInfo* peut faire référence àDirectoryInfo si l'entrée est répertoire.

### Exemples

Composer une archive avec une entrée cryptée compressée LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Voir également

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Créer une entrée unique dans l'archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |
| newEntrySettings | SevenZipEntrySettings | Paramètres de compression et de cryptage utilisés pour les[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Objet. |

### Return_Value

Instance d'entrée de code postal.

### Exemples

Composez une archive 7z avec compression LZMA2 et cryptage de toutes les entrées.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Voir également

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Créer une entrée unique dans l'archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| path | String | Le nom complet du nouveau fichier ou le nom relatif du fichier à compresser. |
| openImmediately | Boolean | Vrai si ouvrir le fichier immédiatement, sinon ouvrir le fichier lors de l'enregistrement de l'archive. |
| newEntrySettings | SevenZipEntrySettings | Paramètres de compression et de cryptage utilisés pour les[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Objet. |

### Return_Value

Instance d'entrée de code postal.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder |
| ArgumentException | La*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Le nom de l'entrée est défini uniquement dans*name* paramètre. Le nom de fichier fourni dans*path* Le paramètre n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec*openImmediately* paramètre, il devient bloqué jusqu'à ce que l'archive soit enregistrée.

### Exemples

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Voir également

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive)
* Assemblée [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
