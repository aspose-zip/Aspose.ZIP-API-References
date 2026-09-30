---
title: "ZstandardArchive.Open"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode ZstandardArchive. Ouvre l'archive pour l'extraction et fournit un flux contenant le contenu de l'archive."
type: docs
weight: 50
url: /fr/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

Ouvre l’archive pour l’extraction et fournit un flux contenant le contenu de l’archive.

```csharp
public Stream Open()
```

### Valeur de retour

Le flux qui représente le contenu de l'archive.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

Lisez le flux pour obtenir le contenu original d'un fichier. Voir la section des exemples.

## Exemples

Extrait l'archive et copie le contenu extrait vers le flux de fichier.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

Vous pouvez utiliser la méthode Stream.CopyTo pour .NET 4.0 et supérieur :

```csharp
unpacked.CopyTo(extracted);
```

### Voir aussi

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


