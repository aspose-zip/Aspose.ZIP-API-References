---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarArchive-Methode. Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu"
type: docs
weight: 30
url: /de/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceDirectory | String | Verzeichnis zum Komprimieren. |
| compressionSettings | Boolean | Die Kompressionseinstellungen, die für hinzugefügte [`XarEntry`](../../xarentry/)‑Elemente verwendet werden. |
| includeRootDirectory | XarCompressionSettings | Gibt an, ob das Stammverzeichnis selbst einbezogen werden soll oder nicht. |

### Rückgabewert

Xar-Eintrag-Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceDirectory* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf *sourceDirectory* zuzugreifen. |
| ArgumentException | *sourceDirectory* enthält ungültige Zeichen wie ", &lt;, &gt;, oder &#x7C;. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beide überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. Der angegebene Pfad, Dateiname oder beide sind zu lang. |
| IOException | *sourceDirectory* steht für eine Datei, nicht für ein Verzeichnis. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Siehe auch

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directory | DirectoryInfo | Verzeichnis zum Komprimieren. |
| compressionSettings | Boolean | Die Kompressionseinstellungen, die für hinzugefügte [`XarEntry`](../../xarentry/)‑Elemente verwendet werden. |
| includeRootDirectory | XarCompressionSettings | Gibt an, ob das Stammverzeichnis selbst einbezogen werden soll oder nicht. |

### Rückgabewert

Xar-Eintrag-Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *directory* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf *directory* zuzugreifen. |
| IOException | *directory* steht für eine Datei, nicht für ein Verzeichnis. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Siehe auch

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


