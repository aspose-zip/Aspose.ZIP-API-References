---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ArchiveFactory-methode. Comprimeert de opgegeven map naar een archiefbestand met behulp van het opgegeven archiefformaat"
type: docs
weight: 10
url: /nl/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Comprimeert de opgegeven map naar een archiefbestand met behulp van het opgegeven archiefformaat.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar de map die zal worden gecomprimeerd. |
| outputFileName | String | Doelbestandsnaam. |
| archiveFormat | ArchiveFormat | Het formaat van het te maken archief (bijv. zip, rar, tar, enz.). |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| DirectoryNotFoundException | Wordt gegooid als de map opgegeven door *path* niet bestaat. |
| ArgumentException | Wordt gegooid als *path* null is of een lege tekenreeks. |
| NotSupportedException | Wordt gegooid als het opgegeven *archiveFormat* niet wordt ondersteund of herkend. |
| ArgumentNullException | *path* is `null`. |

## Opmerkingen

Deze methode maakt een archiefbestand aan op de locatie die is opgegeven door de *path*-parameter. De naam van het archiefbestand is doorgaans de mapnaam gevolgd door de juiste bestandsextensie op basis van *archiveFormat*. De map zelf wordt niet gewijzigd of verwijderd.

## Voorbeelden

Hier is een voorbeeld van hoe de CompressDirectory-methode te gebruiken:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Dit maakt een ZIP-bestand aan met de inhoud van de map op het opgegeven pad.
```

### Zie ook

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


