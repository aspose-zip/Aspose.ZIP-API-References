---
title: "CabArchive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CabArchive-Methode. Speichert das Archiv in den bereitgestellten Stream."
type: docs
weight: 70
url: /de/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Speichert das Archiv in den bereitgestellten Stream.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | Stream | Ziel-Stream. |
| saveOptions | CabSaveOptions | Optionen zum Speichern des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *outputStream* ist nicht schreibbar und suchfähig. |
| ObjectDisposedException | Das Archiv wurde freigegeben. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet und kann nicht gespeichert werden. |

## Hinweise

*outputStream* must be writable.

## Beispiele

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Siehe auch

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Speichert das Archiv in die angegebene Zieldatei.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| saveOptions | CabSaveOptions | Optionen zum Speichern des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *destinationFileName* ist leer, enthält nur Leerzeichen oder enthält ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf die Datei *destinationFileName* wurde verweigert. |
| PathTooLongException | Der angegebene *destinationFileName*, Dateiname oder beide überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Die Datei bei *destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| InvalidOperationException | Das Archiv ist zum Extrahieren geöffnet. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Es ist möglich, ein Archiv am selben Pfad zu speichern, von dem es geladen wurde. Allerdings wird dies nicht empfohlen, da dieser Ansatz das Kopieren in eine temporäre Datei verwendet.

## Beispiele

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Siehe auch

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


