---
title: Archive.Save
second_title: Aspose.ZIP für .NET-API-Referenz
description: Archive methode. Speichert das Archiv im bereitgestellten Stream.
type: docs
weight: 90
url: /de/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Speichert das Archiv im bereitgestellten Stream.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | Stream | Zielstrom. |
| saveOptions | ArchiveSaveOptions | Optionen zum Speichern von Archiven. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *outputStream* ist nicht beschreibbar. |

### Bemerkungen

*outputStream*muss beschreibbar sein.

### Beispiele

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Siehe auch

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Speichert das Archiv in der bereitgestellten Zieldatei.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| saveOptions | ArchiveSaveOptions | Optionen zum Speichern von Archiven. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*destinationFileName* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*destinationFileName* ist abgelehnt. |
| PathTooLongException | Die angegebene*destinationFileName*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Es ist möglich, ein Archiv unter demselben Pfad zu speichern, aus dem es geladen wurde. Dies wird jedoch nicht empfohlen, da dieser Ansatz das Kopieren in eine temporäre Datei verwendet.

### Beispiele

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Siehe auch

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)


