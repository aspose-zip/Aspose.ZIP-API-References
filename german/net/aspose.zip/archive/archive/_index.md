---
title: Archive
second_title: Aspose.ZIP für .NET-API-Referenz
description: Initialisiert eine neue Instanz vonArchiveaspose.zip/archiveKlasse mit optionalen Einstellungen für ihre Einträge.
type: docs
weight: 10
url: /de/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Initialisiert eine neue Instanz von[`Archive`](../../archive)Klasse mit optionalen Einstellungen für ihre Einträge.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für neu hinzugefügte verwendet werden[`ArchiveEntry`](../../archiveentry)items. Wenn nicht angegeben, würde die häufigste Deflate-Komprimierung ohne Verschlüsselung verwendet werden. |

### Beispiele

Das folgende Beispiel zeigt, wie eine einzelne Datei mit Standardeinstellungen komprimiert wird.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Siehe auch

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namensraum [Aspose.Zip](../../archive)
* Montage [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Initialisiert eine neue Instanz von[`Archive`](../../archive) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |
| loadOptions | ArchiveLoadOptions | Optionen zum Laden bestehender Archive mit. |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für neu hinzugefügte verwendet werden[`ArchiveEntry`](../../archiveentry)items. Wenn nicht angegeben, würde die häufigste Deflate-Komprimierung ohne Verschlüsselung verwendet werden. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *sourceStream* ist nicht auffindbar. |
| InvalidDataException | Der Verschlüsselungsheader für AES widerspricht der WinZip-Komprimierungsmethode. |

### Bemerkungen

Dieser Konstruktor dekomprimiert keinen Eintrag. Sehen[`Open`](../../archiveentry/open) Methode zum Dekomprimieren.

### Beispiele

Das folgende Beispiel extrahiert ein verschlüsseltes Archiv und dekomprimiert dann den ersten Eintrag in a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Siehe auch

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namensraum [Aspose.Zip](../../archive)
* Montage [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Initialisiert eine neue Instanz von[`Archive`](../../archive) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der vollständig qualifizierte oder der relative Pfad zur Archivdatei. |
| loadOptions | ArchiveLoadOptions | Optionen zum Laden bestehender Archive mit. |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für neu hinzugefügte verwendet werden[`ArchiveEntry`](../../archiveentry)items. Wenn nicht angegeben, würde die häufigste Deflate-Komprimierung ohne Verschlüsselung verwendet werden. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung |
| ArgumentException | Das*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Dieser Konstruktor dekomprimiert keinen Eintrag. Sehen[`Open`](../../archiveentry/open) Methode zum Dekomprimieren.

### Beispiele

Das folgende Beispiel extrahiert ein verschlüsseltes Archiv und dekomprimiert dann den ersten Eintrag in a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Siehe auch

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namensraum [Aspose.Zip](../../archive)
* Montage [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
