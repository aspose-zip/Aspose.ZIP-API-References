---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarArchive methode. Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.
type: docs
weight: 70
url: /de/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directory | DirectoryInfo | Zu komprimierendes Verzeichnis. |
| includeRootDirectory | Boolean | Gibt an, ob das Stammverzeichnis selbst eingeschlossen werden soll oder nicht. |

### Rückgabewert

Das Archiv mit Einträgen komponiert.

### Beispiele

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceDirectory | String | Zu komprimierendes Verzeichnis. |
| includeRootDirectory | Boolean | Gibt an, ob das Stammverzeichnis selbst eingeschlossen werden soll oder nicht. |

### Rückgabewert

Das Archiv mit Einträgen komponiert.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceDirectory* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung*sourceDirectory*. |
| ArgumentException | *sourceDirectory* enthält ungültige Zeichen wie ", &lt;, &gt; oder &#x7C;. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. Der angegebene Pfad, Dateiname oder beide sind zu lang. |

### Beispiele

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)


