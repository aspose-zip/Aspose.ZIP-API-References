---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Lz4Archive-Methode. Speichert das lz4-Archiv in den bereitgestellten Stream."
type: docs
weight: 60
url: /de/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Speichert das LZ4-Archiv in den angegebenen Stream.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | Stream | Ziel-Stream. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist null. |
| ArgumentException | *output* ist nicht beschreibbar. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet. - oder - Quelle wurde nicht angegeben. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Komprimierung über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

*output* must be seekable.

## Beispiele

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Speichert das LZ4-Archiv in die angegebene Zieldatei.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | FileInfo | FileInfo, das als Ziel-Stream geöffnet wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, das *destination* zu öffnen. |
| ArgumentException | Der Dateipfad ist leer oder enthält nur Leerzeichen. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| UnauthorizedAccessException | Der Pfad zur Datei ist schreibgeschützt oder ein Verzeichnis. |
| ArgumentNullException | *destination* ist null. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Speichert das Archiv in die angegebene Zieldatei.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *destinationFileName* ist leer, enthält nur Leerzeichen oder enthält ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf die Datei *destinationFileName* wurde verweigert. |
| PathTooLongException | Der angegebene *destinationFileName*, Dateiname oder beide überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Die Datei bei *destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig (zum Beispiel, weil er sich auf einem nicht zugeordneten Laufwerk befindet). |
| FileNotFoundException | Die in *destinationFileName* angegebene Datei wurde nicht gefunden. |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |

## Beispiele

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


