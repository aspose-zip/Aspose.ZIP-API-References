---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ArchiveFactory‑Methode. Komprimiert das angegebene Verzeichnis in eine Archivdatei unter Verwendung des angegebenen Archivformats"
type: docs
weight: 10
url: /de/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Komprimiert das angegebene Verzeichnis in eine Archivdatei unter Verwendung des angegebenen Archivformats.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zu dem Verzeichnis, das komprimiert werden soll. |
| outputFileName | String | Zieldateiname. |
| archiveFormat | ArchiveFormat | Das Format des zu erstellenden Archivs (z. B. zip, rar, tar usw.). |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| DirectoryNotFoundException | Wird ausgelöst, wenn das durch *path* angegebene Verzeichnis nicht existiert. |
| ArgumentException | Wird ausgelöst, wenn *path* null oder ein leerer String ist. |
| NotSupportedException | Wird ausgelöst, wenn das angegebene *archiveFormat* nicht unterstützt oder erkannt wird. |
| ArgumentNullException | *path* ist `null`. |

## Hinweise

Diese Methode erstellt eine Archivdatei an dem durch den Parameter *path* angegebenen Ort. Der Name der Archivdatei ist in der Regel der Verzeichnisname, gefolgt von der entsprechenden Dateierweiterung basierend auf *archiveFormat*. Das Verzeichnis selbst wird nicht geändert oder gelöscht.

## Beispiele

Hier ist ein Beispiel, wie man die Methode CompressDirectory verwendet:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Dies erstellt eine ZIP-Datei mit dem Inhalt des Verzeichnisses am angegebenen Pfad.
```

### Siehe auch

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


