---
title: XzArchive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: XzArchive méthode. Enregistre larchive xz dans le flux fourni.
type: docs
weight: 40
url: /fr/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

Enregistre l'archive xz dans le flux fourni.

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
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Voir également

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Enregistre l'archive xz dans le fichier de destination fourni.

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
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### Voir également

* class [XzArchive](../)
* espace de noms [Aspose.Zip.Xz](../../xzarchive/)
* Assemblée [Aspose.Zip](../../../)


