---
title: "CabArchive.CreateEntries"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode CabArchive. Ajoute à l'archive tous les fichiers de manière récursive depuis le répertoire spécifié"
type: docs
weight: 30
url: /fr/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Ajoute à l'archive tous les fichiers, de manière récursive, depuis le répertoire spécifié.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | DirectoryInfo | Répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure le nom du répertoire racine dans les chemins d'entrée. |

### Valeur de retour

L'instance actuelle de [`CabArchive`](../).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* est nul. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| DirectoryNotFoundException | *directory* ne peut pas être trouvé. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder à *directory* ou à son contenu. |
| UnauthorizedAccessException | L'accès à *directory* ou à l'un de ses fichiers est refusé. |
| IOException | Une erreur d'E/S se produit lors de l'accès à *directory*. |
| PathTooLongException | Un chemin d'entrée généré dépasse la longueur maximale définie par le système. |
| InvalidOperationException | L'archive est préparée pour l'extraction et ne peut pas ajouter d'entrées. |

## Exemples

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Voir aussi

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Ajoute à l'archive tous les fichiers de manière récursive depuis le chemin de répertoire spécifié.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Chemin du répertoire à compresser. |
| includeRootDirectory | Boolean | Indique s'il faut inclure le nom du répertoire racine dans les chemins d'entrée. |

### Valeur de retour

L'instance actuelle de [`CabArchive`](../).

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *sourceDirectory* est nul. |
| DirectoryNotFoundException | *sourceDirectory* est introuvable. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder à *sourceDirectory*. |
| UnauthorizedAccessException | L'accès à *sourceDirectory* est refusé. |
| PathTooLongException | Le *sourceDirectory* spécifié dépasse la longueur maximale définie par le système. |
| ArgumentException | *sourceDirectory* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| IOException | Une erreur d'E/S se produit lors de l'accès à *sourceDirectory*. |
| InvalidOperationException | L'archive est préparée pour l'extraction et ne peut pas ajouter d'entrées. |

## Exemples

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Voir aussi

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


