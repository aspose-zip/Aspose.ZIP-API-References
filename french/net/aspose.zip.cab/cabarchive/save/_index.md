---
title: "CabArchive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode CabArchive. Enregistre l'archive dans le flux fourni"
type: docs
weight: 70
url: /fr/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Flux de destination. |
| saveOptions | CabSaveOptions | Options pour l'enregistrement de l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *outputStream* n'est pas inscriptible et déplaçable. |
| ObjectDisposedException | L'archive est libérée. |
| InvalidOperationException | L'archive est préparée pour l'extraction et ne peut pas être enregistrée. |

## Remarques

*outputStream* must be writable.

## Exemples

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Voir aussi

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Enregistre l’archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| saveOptions | CabSaveOptions | Options pour l'enregistrement de l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *destinationFileName* est vide, ne contient que des espaces blancs, ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *destinationFileName* est refusé. |
| PathTooLongException | Le *destinationFileName* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plateformes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichiers moins de 260 caractères. |
| NotSupportedException | Le fichier à *destinationFileName* contient deux-points (:) au milieu de la chaîne. |
| FileNotFoundException | Le fichier est introuvable. |
| InvalidOperationException | L'archive est ouverte pour l'extraction. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

Il est possible d'enregistrer une archive au même chemin d'où elle a été chargée. Cependant, cela n'est pas recommandé car cette approche utilise la copie vers un fichier temporaire.

## Exemples

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Voir aussi

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


