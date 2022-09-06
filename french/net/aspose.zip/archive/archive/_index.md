---
title: Archive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Initialise une nouvelle instance duArchiveaspose.zip/archiveclasse avec des paramètres facultatifs pour ses entrées.
type: docs
weight: 10
url: /fr/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Initialise une nouvelle instance du[`Archive`](../../archive)classe avec des paramètres facultatifs pour ses entrées.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Paramètres de compression et de cryptage utilisés pour les nouveaux[`ArchiveEntry`](../../archiveentry)items. S'il n'est pas spécifié, la compression Deflate la plus courante sans chiffrement sera utilisée. |

### Exemples

L'exemple suivant montre comment compresser un seul fichier avec les paramètres par défaut.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Voir également

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* espace de noms [Aspose.Zip](../../archive)
* Assemblée [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Initialise une nouvelle instance du[`Archive`](../../archive) la liste des entrées de classe et de composition peut être extraite de l'archive.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceStream | Stream | La source des archives. |
| loadOptions | ArchiveLoadOptions | Options pour charger l'archive existante avec. |
| newEntrySettings | ArchiveEntrySettings | Paramètres de compression et de cryptage utilisés pour les nouveaux[`ArchiveEntry`](../../archiveentry)items. S'il n'est pas spécifié, la compression Deflate la plus courante sans chiffrement sera utilisée. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *sourceStream* n'est pas recherchable. |
| InvalidDataException | L'en-tête de chiffrement pour AES contredit la méthode de compression WinZip. |

### Remarques

Ce constructeur ne décompresse aucune entrée. Voir[`Open`](../../archiveentry/open) méthode de décompression.

### Exemples

L'exemple suivant extrait une archive chiffrée, puis décompresse la première entrée dans un`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Voir également

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* espace de noms [Aspose.Zip](../../archive)
* Assemblée [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Initialise une nouvelle instance du[`Archive`](../../archive) la liste des entrées de classe et de composition peut être extraite de l'archive.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès complet ou relatif au fichier d'archive. |
| loadOptions | ArchiveLoadOptions | Options pour charger l'archive existante avec. |
| newEntrySettings | ArchiveEntrySettings | Paramètres de compression et de cryptage utilisés pour les nouveaux[`ArchiveEntry`](../../archiveentry)items. S'il n'est pas spécifié, la compression Deflate la plus courante sans chiffrement sera utilisée. |

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

Ce constructeur ne décompresse aucune entrée. Voir[`Open`](../../archiveentry/open) méthode de décompression.

### Exemples

L'exemple suivant extrait une archive chiffrée, puis décompresse la première entrée dans un`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Voir également

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* espace de noms [Aspose.Zip](../../archive)
* Assemblée [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
