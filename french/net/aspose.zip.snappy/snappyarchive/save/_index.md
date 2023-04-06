---
title: SnappyArchive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SnappyArchive méthode. Enregistre larchive rapide dans le flux fourni.
type: docs
weight: 40
url: /fr/net/aspose.zip.snappy/snappyarchive/save/
---
## Save(Stream) {#save_1}

Enregistre l'archive rapide dans le flux fourni.

```csharp
public void Save(Stream output)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| output | Stream | Flux de destination. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *output* ne supporte pas la recherche. |
| ArgumentNullException | *output* est nul. |

### Remarques

*output* doit être recherchable.

### Exemples

```csharp
using (FileStream snappyFile = File.Open("archive.snappy", FileMode.Create))
{
    using (var archive = new SnappyArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(snappyFile);
     }
}
```

### Voir également

* class [SnappyArchive](../)
* espace de noms [Aspose.Zip.Snappy](../../snappyarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Enregistre l'archive rapide dans le fichier de destination fourni.

```csharp
public void Save(FileInfo destination)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destination | FileInfo | FileInfo qui sera ouvert en tant que flux de destination. |

### Exceptions

| exception | condition |
| --- | --- |
| SecurityException | L'appelant n'a pas l'autorisation requise pour ouvrir le*destination*. |
| ArgumentException | Le chemin du fichier est vide ou ne contient que des espaces blancs. |
| FileNotFoundException | Le fichier est introuvable. |
| UnauthorizedAccessException | Le chemin d'accès au fichier est en lecture seule ou est un répertoire. |
| ArgumentNullException | *destination* est nul. |
| DirectoryNotFoundException | Le chemin spécifié n'est pas valide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |

### Exemples

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.snappy"));
}
```

### Voir également

* class [SnappyArchive](../)
* espace de noms [Aspose.Zip.Snappy](../../snappyarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Enregistre l'archive rapide dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |

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

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.snappy");
}
```

### Voir également

* class [SnappyArchive](../)
* espace de noms [Aspose.Zip.Snappy](../../snappyarchive/)
* Assemblée [Aspose.Zip](../../../)


