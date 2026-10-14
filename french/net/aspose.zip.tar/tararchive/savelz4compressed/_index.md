---
title: "TarArchive.SaveLZ4Compressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode TarArchive. Enregistre l'archive dans le flux avec compression LZ4"
type: docs
weight: 170
url: /fr/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

Enregistre l'archive dans le flux avec compression LZ4.

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | Stream | Flux de destination. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas accessible en écriture. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée |
| IOException | Une erreur d'E/S se produit. |

## Remarques

*output* must be writable.

## Exemples

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### Voir aussi

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

Enregistre l'archive dans le fichier par chemin avec compression LZ4.

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible. |

### Exceptions

| exception | condition |
| --- | --- |
| UnauthorizedAccessException | L'appelant ne possède pas l'autorisation requise. -ou- *path* indique un fichier ou répertoire en lecture seule. |
| ArgumentException | *path* est une chaîne de longueur zéro, ne contient que des espaces blancs, ou contient un ou plusieurs caractères invalides tels que définis par InvalidPathChars. |
| ArgumentNullException | *path* est nul. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| DirectoryNotFoundException | Le *path* spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| NotSupportedException | *path* est dans un format invalide. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée |
| IOException | Une erreur d'E/S se produit. |

## Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### Voir aussi

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


