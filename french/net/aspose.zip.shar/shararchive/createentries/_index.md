---
title: SharArchive.CreateEntries
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SharArchive méthode. Ajoute à larchive tous les fichiers et répertoires de manière récursive dans le répertoire donné.
type: docs
weight: 30
url: /fr/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceDirectory | String | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure ou non le répertoire racine lui-même. |

### Return_Value

Instance d'entrée Shar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceDirectory* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder*sourceDirectory*. |
| ArgumentException | *sourceDirectory* contient des caractères non valides tels que ", &lt;, &gt; ou &#x7C;. |
| PathTooLongException | Le chemin d'accès, le nom de fichier ou les deux spécifiés dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. Le chemin d'accès spécifié, le nom de fichier ou les deux sont trop longs. |
| IOException | *sourceDirectory* représente un fichier, pas un répertoire. |

### Exemples

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Voir également

* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| directory | DirectoryInfo | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure ou non le répertoire racine lui-même. |

### Return_Value

Instance d'entrée Shar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder*directory*. |
| IOException | *directory* représente un fichier, pas un répertoire. |

### Exemples

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Voir également

* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)


