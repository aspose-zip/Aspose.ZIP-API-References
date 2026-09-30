---
title: "TarArchive.FromLZMA"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "TarArchive-Methode. Extrahiert das bereitgestellte LZMA-Archiv und erstellt ein TarArchive aus den extrahierten Daten."
type: docs
weight: 50
url: /de/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Extrahiert das bereitgestellte LZMA-Archiv und erstellt [`TarArchive`](../) aus den extrahierten Daten.

Wichtig: Das LZMA-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quelle | Stream | Die Quelle des Archivs. |

### Rückgabewert

Eine Instanz von [`TarArchive`](../)

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidDataException | Das Archiv ist beschädigt. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams erreicht wird, bevor die erwartete Anzahl von Bytes gelesen wurde. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| ArgumentNullException | *source* ist null. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Hinweise

Der LZMA-Extraktionsstrom ist aufgrund der Natur des Kompressionsalgorithmus nicht seekbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen seekbaren Stream verwenden muss.

### Siehe auch

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Extrahiert das bereitgestellte LZMA-Archiv und erstellt [`TarArchive`](../) aus den extrahierten Daten.

Wichtig: Das LZMA-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

```csharp
public static TarArchive FromLZMA(string path)
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
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei unter *path* hat ein ungültiges Format. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams erreicht wird, bevor die erwartete Anzahl von Bytes gelesen wurde. |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |
| InvalidDataException | Das Archiv ist beschädigt. |

## Hinweise

Der LZMA-Extraktionsstrom ist aufgrund der Natur des Kompressionsalgorithmus nicht seekbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen seekbaren Stream verwenden muss.

### Siehe auch

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


