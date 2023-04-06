---
title: Archive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Archive méthode. Enregistre larchive dans le flux fourni.
type: docs
weight: 90
url: /fr/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| outputStream | Stream | Flux de destination. |
| saveOptions | ArchiveSaveOptions | Options de sauvegarde des archives. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *outputStream* n'est pas inscriptible. |

### Remarques

*outputStream*doit être inscriptible.

### Exemples

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Voir également

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* espace de noms [Aspose.Zip](../../archive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| saveOptions | ArchiveSaveOptions | Options de sauvegarde des archives. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*destinationFileName* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*destinationFileName* est refusé. |
| PathTooLongException | Le spécifié*destinationFileName*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plateformes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*destinationFileName* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Il est possible d'enregistrer une archive dans le même chemin que celui depuis lequel elle a été chargée. Cependant, cela n'est pas recommandé car cette approche utilise la copie dans un fichier temporaire.

### Exemples

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Voir également

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* espace de noms [Aspose.Zip](../../archive/)
* Assemblée [Aspose.Zip](../../../)


