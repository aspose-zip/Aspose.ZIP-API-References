---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode CpioArchive. Enregistre l'archive dans le flux avec compression LZMA."
type: docs
weight: 110
url: /fr/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Enregistre l'archive dans le flux avec une compression LZMA.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | Stream | Flux de destination. |
| cpioFormat | CpioFormat | Définit le format d'en-tête cpio. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| NotSupportedException | Le flux ne prend pas en charge l'écriture, ou le flux est déjà fermé. |

## Remarques

*output* must be writable.

Important : l'archive cpio est composée puis compressée dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

## Exemples

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
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

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Enregistre l'archive dans le fichier par chemin avec une compression lzma.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| Exception | Lancée lorsqu'une erreur d'exécution se produit. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| IOException | Une erreur d'E/S se produit. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. |
| UnauthorizedAccessException | L'appelant ne possède pas l'autorisation requise. -ou- *path* indique un fichier ou répertoire en lecture seule. |

## Remarques

Important : l'archive cpio est composée puis compressée dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

## Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Voir aussi

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


