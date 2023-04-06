---
title: Archive.CreateEntries
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Archive méthode. Ajoute à larchive tous les fichiers et répertoires de manière récursive dans le répertoire donné.
type: docs
weight: 40
url: /fr/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| directory | DirectoryInfo | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure ou non le répertoire racine lui-même. |

### Return_Value

L'archive avec des entrées composées.

### Exceptions

| exception | condition |
| --- | --- |
| DirectoryNotFoundException | Le chemin vers*directory* n'est pas valide, par exemple s'il se trouve sur un lecteur non mappé. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder*directory*. |

### Exemples

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Voir également

* class [Archive](../)
* espace de noms [Aspose.Zip](../../archive/)
* Assemblée [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceDirectory | String | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure ou non le répertoire racine lui-même. |

### Return_Value

L'archive avec des entrées composées.

### Exemples

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Voir également

* class [Archive](../)
* espace de noms [Aspose.Zip](../../archive/)
* Assemblée [Aspose.Zip](../../../)


