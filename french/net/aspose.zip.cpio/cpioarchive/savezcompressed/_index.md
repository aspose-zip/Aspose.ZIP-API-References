---
title: "CpioArchive.SaveZCompressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode CpioArchive. Enregistre l'archive dans le flux avec compression Z."
type: docs
weight: 130
url: /fr/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Enregistre l'archive dans le flux avec compression Z.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | Stream | Flux de destination. |
| cpioFormat | CpioFormat | Définit le format d'en-tête cpio. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas accessible en écriture. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

*output* must be writable.

## Exemples

```csharp
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
        }
    }
}
```

### Voir aussi

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Enregistre l'archive sur le chemin par chemin avec compression Z.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| cpioFormat | CpioFormat | Définit le format d'en-tête cpio. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *path* est `null`. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| IOException | Une erreur d'E/S se produit. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. |

## Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Voir aussi

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


