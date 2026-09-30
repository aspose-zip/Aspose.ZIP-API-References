---
title: "XarArchive.CreateEntries"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode XarArchive. Ajoute à l'archive tous les fichiers et répertoires de façon récursive dans le répertoire donné"
type: docs
weight: 30
url: /fr/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Ajoute à l'archive tous les fichiers et répertoires de façon récursive dans le répertoire donné.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Répertoire à compresser. |
| compressionSettings | Boolean | Les paramètres de compression utilisés pour les éléments [`XarEntry`](../../xarentry/) ajoutés. |
| includeRootDirectory | XarCompressionSettings | Indique s'il faut inclure le répertoire racine lui-même ou non. |

### Valeur de retour

Instance d'entrée Xar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceDirectory* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder à *sourceDirectory*. |
| ArgumentException | *sourceDirectory* contient des caractères invalides tels que ", &lt;, &gt;, ou &#x7C;. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères, et les noms de fichier moins de 260 caractères. Le chemin spécifié, le nom de fichier, ou les deux sont trop longs. |
| IOException | *sourceDirectory* représente un fichier, pas un répertoire. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Voir aussi

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Ajoute à l'archive tous les fichiers et répertoires de façon récursive dans le répertoire donné.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | DirectoryInfo | Répertoire à compresser. |
| compressionSettings | Boolean | Les paramètres de compression utilisés pour les éléments [`XarEntry`](../../xarentry/) ajoutés. |
| includeRootDirectory | XarCompressionSettings | Indique s'il faut inclure le répertoire racine lui-même ou non. |

### Valeur de retour

Instance d'entrée Xar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder à *directory*. |
| IOException | *directory* représente un fichier, pas un répertoire. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Voir aussi

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


