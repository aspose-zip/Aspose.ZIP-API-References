---
title: "UueArchive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "UueArchive-Methode. Speichert das Archiv in den bereitgestellten Stream."
type: docs
weight: 70
url: /de/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Speichert das Archiv in den bereitgestellten Stream.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | Stream | Ziel-Stream. |
| saveOptions | UueSaveOptions | Optionen für das Speichern des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Die Quelle der zu archivierenden Daten wurde nicht angegeben. |
| ArgumentException | *outputStream* ist nicht beschreibbar. |
| UnauthorizedAccessException | Dateiquelle ist schreibgeschützt oder ein Verzeichnis. |
| DirectoryNotFoundException | Der angegebene Pfad der Dateiquelle ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Dateiquelle ist bereits geöffnet. |

## Hinweise

*outputStream* must be writable.

## Beispiele

Komprimierte Daten in den HTTP-Antwort-Stream schreiben.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Siehe auch

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Speichert das Archiv in eine bereitgestellte Zieldatei.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| saveOptions | UueSaveOptions | Optionen für das Speichern des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *destinationFileName* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *destinationFileName* ist leer, enthält nur Leerzeichen oder enthält ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf die Datei *destinationFileName* wurde verweigert. |
| PathTooLongException | Der angegebene *destinationFileName*, Dateiname oder beide überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Die Datei bei *destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| InvalidOperationException | Die Quelle der zu archivierenden Daten wurde nicht angegeben. |

## Beispiele

Kodierte Daten in die Datei schreiben.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Siehe auch

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


