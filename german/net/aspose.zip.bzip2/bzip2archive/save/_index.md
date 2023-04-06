---
title: Bzip2Archive.Save
second_title: Aspose.ZIP für .NET-API-Referenz
description: Bzip2Archive methode. Speichert das Archiv im bereitgestellten Stream.
type: docs
weight: 50
url: /de/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Speichert das Archiv im bereitgestellten Stream.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | Stream | Zielstrom. |
| saveOptions | Bzip2SaveOptions | Optionen zum Speichern eines bzip2-Archivs. Wenn nicht angegeben, wird eine Blockgröße von 900 KB verwendet. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Die Quelle der zu archivierenden Daten wurde nicht angegeben. |
| ArgumentException | *outputStream* ist nicht beschreibbar. |
| UnauthorizedAccessException | Die Dateiquelle ist schreibgeschützt oder ein Verzeichnis. |
| DirectoryNotFoundException | Der angegebene Dateiquellpfad ist ungültig, da er sich beispielsweise auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Dateiquelle ist bereits geöffnet. |

### Bemerkungen

*outputStream*muss beschreibbar sein.

### Beispiele

Schreibt komprimierte Daten in den HTTP-Antwortstrom.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Siehe auch

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Speichert das Archiv in der bereitgestellten Zieldatei.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| saveOptions | Bzip2SaveOptions | Optionen zum Speichern eines bzip2-Archivs. Wenn nicht angegeben, wird eine Blockgröße von 900 KB verwendet. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*destinationFileName* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*destinationFileName* ist abgelehnt. |
| PathTooLongException | Die angegebene*destinationFileName*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Beispiele

Schreibt komprimierte Daten in eine Datei.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Siehe auch

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)


