---
title: "IsoArchive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode IsoArchive. Enregistre l'image ISO à l'emplacement spécifié"
type: docs
weight: 70
url: /fr/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Enregistre l'image ISO dans le chemin spécifié.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin où l'image ISO sera enregistrée. |
| saveOptions | IsoSaveOptions | Options pour enregistrer l'archive ISO. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Lancé lorsque l'archive n'est pas en mode édition. |
| ArgumentNullException | Lancé lorsque *path* est nul. |
| DirectoryNotFoundException | Lancé lorsque le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Lancé lorsque le fichier est déjà ouvert. |
| UnauthorizedAccessException | Lancé lorsque l'accès au fichier *path* est refusé. |
| PathTooLongException | Lancé lorsque le *path* spécifié dépasse la longueur maximale définie par le système. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

L'exemple suivant montre comment enregistrer une archive ISO dans un fichier :

```csharp
// Créer une nouvelle archive ISO vide
using(IsoArchive isoArchive = new IsoArchive())
{
    // Ajouter des fichiers à l'archive ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Enregistrer l'archive ISO dans un fichier
    isoArchive.Save("new_archive.iso");
}
```

### Voir aussi

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Enregistre l'image ISO dans le flux spécifié.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux où l'image ISO sera enregistrée. |
| saveOptions | IsoSaveOptions | Options pour enregistrer l'archive ISO. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Lancé lorsque l'archive n'est pas en mode édition. |
| ArgumentNullException | Lancé lorsque le *stream* est nul. |
| ArgumentException | Lancée lorsque le *stream* n'est pas accessible en écriture. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| IOException | Une erreur d'E/S se produit. |

## Exemples

L'exemple suivant montre comment enregistrer une archive ISO dans un flux mémoire :

```csharp

 // Créer une nouvelle archive ISO vide
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Ajouter des fichiers à l'archive ISO
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Enregistrer l'archive ISO dans un flux mémoire
     isoArchive.Save(memoryStream);
 }
```

### Voir aussi

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


