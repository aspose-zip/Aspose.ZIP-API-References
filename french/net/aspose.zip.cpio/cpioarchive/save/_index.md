---
title: CpioArchive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: CpioArchive méthode. Enregistre larchive dans le fichier de destination fourni.
type: docs
weight: 80
url: /fr/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| cpioFormat | CpioFormat | Définit le format d'en-tête cpio. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destinationFileName* est une chaîne de longueur nulle, ne contient que des espaces blancs ou contient un ou plusieurs caractères non valides tels que définis par System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* est nul. |
| PathTooLongException | Le spécifié*destinationFileName*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| DirectoryNotFoundException | Le spécifié*destinationFileName* n'est pas valide (par exemple, il se trouve sur un lecteur non mappé). |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |
| UnauthorizedAccessException | *destinationFileName* a spécifié un fichier en lecture seule et l'accès n'est pas en lecture.-ou- chemin a spécifié un répertoire.-ou- L'appelant n'a pas l'autorisation requise. |
| NotSupportedException | *destinationFileName* est dans un format invalide. |

### Remarques

Il est possible d'enregistrer une archive dans le même chemin que celui depuis lequel elle a été chargée. Cependant, cela n'est pas recommandé car cette approche utilise la copie dans un fichier temporaire.

### Exemples

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Voir également

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| output | Stream | Flux de destination. |
| cpioFormat | CpioFormat | Définit le format d'en-tête cpio. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas inscriptible. - ou -*output* est le même flux dont nous extrayons. - OU - Il est impossible d'enregistrer l'archive dans*cpioFormat* en raison des restrictions de format. |

### Remarques

*output*doit être inscriptible.

### Exemples

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Voir également

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)


