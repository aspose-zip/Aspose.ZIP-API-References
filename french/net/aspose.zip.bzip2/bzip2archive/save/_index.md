---
title: Bzip2Archive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Bzip2Archive méthode. Enregistre larchive dans le flux fourni.
type: docs
weight: 50
url: /fr/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| outputStream | Stream | Flux de destination. |
| saveOptions | Bzip2SaveOptions | Options de sauvegarde d'une archive bzip2. S'il n'est pas spécifié, une taille de bloc de 900 Ko sera utilisée. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | La source des données à archiver n'a pas été fournie. |
| ArgumentException | *outputStream* n'est pas inscriptible. |
| UnauthorizedAccessException | La source du fichier est en lecture seule ou est un répertoire. |
| DirectoryNotFoundException | Le chemin d'accès source du fichier spécifié n'est pas valide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | La source du fichier est déjà ouverte. |

### Remarques

*outputStream*doit être inscriptible.

### Exemples

Écrit les données compressées dans le flux de réponse http.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Voir également

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| saveOptions | Bzip2SaveOptions | Options de sauvegarde d'une archive bzip2. S'il n'est pas spécifié, une taille de bloc de 900 Ko sera utilisée. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*destinationFileName* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*destinationFileName* est refusé. |
| PathTooLongException | Le spécifié*destinationFileName*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*destinationFileName* contient deux-points (:) au milieu de la chaîne. |

### Exemples

Écrit les données compressées dans le fichier.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Voir également

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)


