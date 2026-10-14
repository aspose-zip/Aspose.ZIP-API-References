---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoEntry Methode. Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad"
type: docs
weight: 50
url: /de/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

### Rückgabewert

FileInfo-Instanz, die extrahierte Daten enthält.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| InvalidOperationException | Archivköpfe und Serviceinformationen wurden nicht gelesen. |

### Siehe auch

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrahiert den Eintrag in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| NotSupportedException | Wird ausgelöst, wenn der Eintrag keine Datei darstellt. |
| ArgumentException | Der bereitgestellte Stream unterstützt das Schreiben nicht. |

### Siehe auch

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


