---
title: CpioArchive.CreateEntries
second_title: Aspose.ZIP für .NET-API-Referenz
description: CpioArchive methode. Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.
type: docs
weight: 30
url: /de/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceDirectory | String | Zu komprimierendes Verzeichnis. |
| includeRootDirectory | Boolean | Gibt an, ob das Stammverzeichnis selbst eingeschlossen werden soll oder nicht. |

### Rückgabewert

Cpio-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceDirectory* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung*sourceDirectory*. |
| ArgumentException | *sourceDirectory* enthält ungültige Zeichen wie ", &lt;, &gt; oder &#x7C;. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. Der angegebene Pfad, Dateiname oder beide sind zu lang. |
| IOException | *sourceDirectory* steht für eine Datei, nicht für ein Verzeichnis. |

### Beispiele

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### Siehe auch

* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directory | DirectoryInfo | Zu komprimierendes Verzeichnis. |
| includeRootDirectory | Boolean | Gibt an, ob das Stammverzeichnis selbst eingeschlossen werden soll oder nicht. |

### Rückgabewert

Cpio-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *directory* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung*directory*. |
| IOException | *directory* steht für eine Datei, nicht für ein Verzeichnis. |

### Beispiele

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### Siehe auch

* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)


