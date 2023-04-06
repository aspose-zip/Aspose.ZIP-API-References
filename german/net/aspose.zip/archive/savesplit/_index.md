---
title: Archive.SaveSplit
second_title: Aspose.ZIP für .NET-API-Referenz
description: Archive methode. Speichert mehrvolumiges Archiv im angegebenen Zielverzeichnis.
type: docs
weight: 100
url: /de/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Speichert mehrvolumiges Archiv im angegebenen Zielverzeichnis.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | String | Der Pfad zu dem Verzeichnis, in dem Archivsegmente erstellt werden sollen. |
| options | SplitArchiveSaveOptions | Optionen zum Speichern des Archivs, einschließlich Dateiname. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Dieses Archiv wurde aus einer vorhandenen Quelle geöffnet. |
| NotSupportedException | Dieses Archiv ist sowohl mit der XZ-Methode komprimiert als auch verschlüsselt. |
| ArgumentNullException | *destinationDirectory* ist Null. |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung, auf das Verzeichnis zuzugreifen. |
| ArgumentException | *destinationDirectory* enthält ungültige Zeichen wie ", &gt;, &lt; oder &#x7C;. |
| PathTooLongException | Der angegebene Pfad überschreitet die vom System definierte maximale Länge. |

### Bemerkungen

Diese Methode besteht aus mehreren (`N`) Dateien Dateiname.z01, Dateiname.z02, ..., Dateiname.z(n-1), Dateiname.zip.

Vorhandenes Archiv kann nicht in mehrere Volumes umgewandelt werden.

### Beispiele

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Siehe auch

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)


