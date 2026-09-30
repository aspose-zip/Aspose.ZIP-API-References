---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CabArchive‑Methode. Fügt dem Archiv alle Dateien rekursiv aus dem angegebenen Verzeichnis hinzu"
type: docs
weight: 30
url: /de/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Fügt dem Archiv alle Dateien, rekursiv, aus dem angegebenen Verzeichnis hinzu.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directory | DirectoryInfo | Verzeichnis zum Komprimieren. |
| includeRootDirectory | Boolean | Gibt an, ob der Name des Stammverzeichnisses in den Eintragspfaden enthalten sein soll. |

### Rückgabewert

Die aktuelle [`CabArchive`](../)‑Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *directory* ist null. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| DirectoryNotFoundException | *directory* kann nicht gefunden werden. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf *directory* oder dessen Inhalt zuzugreifen. |
| UnauthorizedAccessException | Der Zugriff auf *directory* oder eine seiner Dateien wurde verweigert. |
| IOException | Beim Zugriff auf *directory* tritt ein I/O-Fehler auf. |
| PathTooLongException | Ein generierter Eintragspfad überschreitet die systemdefinierte maximale Länge. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet und kann keine Einträge hinzufügen. |

## Beispiele

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Siehe auch

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Fügt dem Archiv alle Dateien rekursiv aus dem angegebenen Verzeichnispfad hinzu.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceDirectory | String | Verzeichnispfad zum Komprimieren. |
| includeRootDirectory | Boolean | Gibt an, ob der Name des Stammverzeichnisses in den Eintragspfaden enthalten sein soll. |

### Rückgabewert

Die aktuelle [`CabArchive`](../)‑Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *sourceDirectory* ist null. |
| DirectoryNotFoundException | *sourceDirectory* kann nicht gefunden werden. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf *sourceDirectory* zuzugreifen. |
| UnauthorizedAccessException | Zugriff auf *sourceDirectory* wurde verweigert. |
| PathTooLongException | Das angegebene *sourceDirectory* überschreitet die systemdefinierte maximale Länge. |
| ArgumentException | *sourceDirectory* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| IOException | Beim Zugriff auf *sourceDirectory* tritt ein I/O-Fehler auf. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet und kann keine Einträge hinzufügen. |

## Beispiele

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Siehe auch

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


