---
title: "CpioArchive.SaveZstandard"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode CpioArchive. Enregistre l'archive dans le flux avec compression Zstandard."
type: docs
weight: 140
url: /fr/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Enregistre l'archive dans le flux avec compression Zstandard.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Enregistre l'archive dans le fichier par chemin avec la compression Zstandard.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| cpioFormat | CpioFormat | Définit le format d'en-tête cpio. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentException | *path* est une chaîne de longueur zéro, ne contient que des espaces blancs, ou contient un ou plusieurs caractères invalides tels que définis par InvalidPathChars. |
| ArgumentNullException | *path* est `null`. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| IOException | Une erreur d'E/S se produit. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. |
| UnauthorizedAccessException | L'appelant ne possède pas l'autorisation requise. -ou- *path* indique un fichier ou répertoire en lecture seule. |

## Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Voir aussi

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


