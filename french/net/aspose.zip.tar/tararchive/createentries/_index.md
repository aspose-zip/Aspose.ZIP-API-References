---
title: TarArchive.CreateEntries
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Ajoute à larchive tous les fichiers et répertoires de manière récursive dans le répertoire donné.
type: docs
weight: 70
url: /fr/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| directory | DirectoryInfo | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure ou non le répertoire racine lui-même. |

### Return_Value

L'archive avec des entrées composées.

### Exemples

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceDirectory | String | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure ou non le répertoire racine lui-même. |

### Return_Value

L'archive avec des entrées composées.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceDirectory* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder*sourceDirectory*. |
| ArgumentException | *sourceDirectory* contient des caractères non valides tels que ", &lt;, &gt; ou &#x7C;. |
| PathTooLongException | Le chemin d'accès, le nom de fichier ou les deux spécifiés dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. Le chemin d'accès spécifié, le nom de fichier ou les deux sont trop longs. |

### Exemples

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


