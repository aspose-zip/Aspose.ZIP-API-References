---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipArchive methode. Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.
type: docs
weight: 40
url: /de/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directory | DirectoryInfo | Zu komprimierendes Verzeichnis. |
| includeRootDirectory | Boolean | Gibt an, ob das Stammverzeichnis selbst eingeschlossen werden soll oder nicht. |

### Rückgabewert

Das Archiv mit Einträgen komponiert.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| DirectoryNotFoundException | Der Weg zu*directory* ungültig ist, z. B. auf einem nicht zugeordneten Laufwerk. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung*directory*. |

### Beispiele

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Siehe auch

* class [SevenZipArchive](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Montage [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceDirectory | String | Zu komprimierendes Verzeichnis. |
| includeRootDirectory | Boolean | Gibt an, ob das Stammverzeichnis selbst eingeschlossen werden soll oder nicht. |

### Rückgabewert

Das Archiv mit Einträgen komponiert.

### Beispiele

Erstellen Sie ein 7z-Archiv mit LZMA2-Komprimierung.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Siehe auch

* class [SevenZipArchive](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Montage [Aspose.Zip](../../../)


