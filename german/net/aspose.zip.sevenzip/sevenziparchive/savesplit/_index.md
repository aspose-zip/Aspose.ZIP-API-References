---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipArchive methode. Speichert mehrvolumiges Archiv im angegebenen Zielverzeichnis.
type: docs
weight: 90
url: /de/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Speichert mehrvolumiges Archiv im angegebenen Zielverzeichnis.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | String | Der Pfad zu dem Verzeichnis, in dem Archivsegmente erstellt werden sollen. |
| options | SplitSevenZipArchiveSaveOptions | Optionen zum Speichern des Archivs, einschließlich Dateiname. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Dieses Archiv wurde aus einer vorhandenen Quelle geöffnet. |
| ArgumentNullException | *destinationDirectory* ist Null. |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung, auf das Verzeichnis zuzugreifen. |
| ArgumentException | *destinationDirectory* enthält ungültige Zeichen wie ", &gt;, &lt; oder &#x7C;. |
| PathTooLongException | Der angegebene Pfad überschreitet die vom System definierte maximale Länge. |

### Bemerkungen

Diese Methode besteht aus mehreren (`N`) Dateien Dateiname.7z.001, Dateiname.7z.002, ..., Dateiname.7z.(n).

Vorhandenes Archiv kann nicht in mehrere Volumes umgewandelt werden.

### Beispiele

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Siehe auch

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Montage [Aspose.Zip](../../../)


