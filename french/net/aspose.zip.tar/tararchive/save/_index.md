---
title: TarArchive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Enregistre larchive dans le flux fourni.
type: docs
weight: 120
url: /fr/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| output | Stream | Flux de destination. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur nulle sera traitée comme UStar lorsque cela est possible. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *output* n'est pas inscriptible. - ou -*output* est le même flux dont nous extrayons. - OU - Il est impossible d'enregistrer l'archive dans*format* en raison des restrictions de format. |

### Remarques

*output*doit être inscriptible.

### Exemples

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur nulle sera traitée comme UStar lorsque cela est possible. |

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
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


