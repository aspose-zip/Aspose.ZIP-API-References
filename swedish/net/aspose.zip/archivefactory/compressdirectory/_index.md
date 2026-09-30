---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ArchiveFactory‑metod. Komprimerar den angivna katalogen till en arkivfil med det angivna arkivformatet"
type: docs
weight: 10
url: /sv/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Komprimerar den angivna katalogen till en arkivfil med det angivna arkivformatet.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till katalogen som ska komprimeras. |
| outputFileName | String | Destinationsfilnamn. |
| archiveFormat | ArchiveFormat | Formatet på arkivet som ska skapas (t.ex. zip, rar, tar, osv.). |

### Undantag

| undantag | villkor |
| --- | --- |
| DirectoryNotFoundException | Kastas om katalogen som anges av *path* inte finns. |
| ArgumentException | Kastas om *path* är null eller en tom sträng. |
| NotSupportedException | Kastas om det angivna *archiveFormat* inte stöds eller känns igen. |
| ArgumentNullException | *path* är `null`. |

## Anmärkningar

Denna metod kommer att skapa en arkivfil på den plats som anges av parametern *path*. Arkivfilens namn kommer vanligtvis att vara katalognamnet följt av rätt filändelse baserat på *archiveFormat*. Katalogen själv ändras eller tas inte bort.

## Exempel

Här är ett exempel på hur man använder metoden CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Detta kommer att skapa en ZIP-fil med innehållet i katalogen på den angivna sökvägen.
```

### Se även

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


