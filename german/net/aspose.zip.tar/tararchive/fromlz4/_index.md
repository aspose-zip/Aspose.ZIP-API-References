---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "TarArchive-Methode. Extrahiert das bereitgestellte LZ4-Archiv und erstellt ein TarArchive aus den extrahierten Daten"
type: docs
weight: 30
url: /de/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Extrahiert das bereitgestellte LZ4-Archiv und erstellt [`TarArchive`](../) aus den extrahierten Daten.

Wichtig: Das LZ4-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern behalten. Achten Sie auf den Speicherverbrauch.

```csharp
public static TarArchive FromLZ4(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Archivdatei. |

### Rückgabewert

Eine Instanz von [`TarArchive`](../)

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei unter *path* hat ein ungültiges Format. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| EndOfStreamException | Die Datei ist zu kurz. |
| InvalidDataException | Die Datei hat die falsche Signatur. |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |
| InvalidOperationException | Das Archiv ist für die Zusammensetzung vorbereitet. |

## Hinweise

Der LZ4-Extraktionsstream ist aufgrund der Natur des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, daher muss es intern einen suchbaren Stream verwenden.

### Siehe auch

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Extrahiert das bereitgestellte LZ4-Archiv und erstellt [`TarArchive`](../) aus den extrahierten Daten.

Wichtig: Das LZ4-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern behalten. Achten Sie auf den Speicherverbrauch.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quelle | Stream | Die Quelle des Archivs. |

### Rückgabewert

Eine Instanz von [`TarArchive`](../)

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Kann nicht von *source* lesen |
| ArgumentNullException | *source* ist null. |
| EndOfStreamException | *source* ist zu kurz. |
| InvalidDataException | Die *source* hat die falsche Signatur. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |

## Hinweise

Der LZ4-Extraktionsstream ist aufgrund der Natur des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, daher muss es intern einen suchbaren Stream verwenden.

### Siehe auch

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


