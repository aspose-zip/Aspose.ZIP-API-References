---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "UueArchive-Konstruktor. Initialisiert eine neue Instanz der UueArchive-Klasse, die für das Kodieren vorbereitet ist"
type: docs
weight: 10
url: /de/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Initialisiert eine neue Instanz der [`UueArchive`](../)-Klasse, die für das Kodieren vorbereitet ist.

```csharp
public UueArchive()
```

## Beispiele

Das folgende Beispiel zeigt, wie man eine Datei uuencodiert.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Siehe auch

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Initialisiert eine neue Instanz der [`UueArchive`](../)-Klasse, die für das Dekodieren vorbereitet ist.

```csharp
public UueArchive(Stream sourceStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |

## Hinweise

Dieser Konstruktor dekodiert nicht. Siehe die [`Open`](../open/)-Methode zum Dekomprimieren.

## Beispiele

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in einen `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Initialisiert eine neue Instanz der [`UueArchive`](../)-Klasse.

```csharp
public UueArchive(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Archivdatei. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| IOException | Die Datei ist bereits geöffnet. |

## Hinweise

Dieser Konstruktor dekomprimiert nicht. Siehe die [`Open`](../open/)-Methode zum Dekomprimieren.

## Beispiele

Öffnen Sie ein Archiv aus einer Datei über den Pfad und dekodieren Sie es in einen `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


