---
title: "UueArchive.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "UueArchive-Methode. Extrahiert das Archiv in den bereitgestellten Stream"
type: docs
weight: 40
url: /de/net/aspose.zip.uue/uuearchive/extract/
---
## Extract(Stream) {#extract_1}

Extrahiert das Archiv in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |

## Beispiele

```csharp
using (var archive = new UueArchive("archive.uue"))
{
     archive.Extract(httpResponseStream);
}
```

### Siehe auch

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrahiert das Archiv in die Datei über den Pfad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

### Rückgabewert

Informationen der extrahierten Datei.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| InvalidDataException | Wird ausgelöst, wenn die Daten ungültig oder beschädigt sind. |

### Siehe auch

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


