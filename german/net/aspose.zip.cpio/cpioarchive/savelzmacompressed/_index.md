---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CpioArchive-Methode. Speichert das Archiv in den Stream mit LZMA-Kompression."
type: docs
weight: 110
url: /de/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Speichert das Archiv mit LZMA-Kompression im Stream.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | Stream | Ziel-Stream. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| NotSupportedException | Der Stream unterstützt kein Schreiben oder ist bereits geschlossen. |

## Hinweise

*output* must be writable.

Wichtig: Das cpio-Archiv wird in dieser Methode erstellt und anschließend komprimiert, sein Inhalt wird intern gehalten. Achtung bei Speicherverbrauch.

## Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Speichert das Archiv über den Pfad mit lzma-Kompression in einer Datei.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *path* ist `null`. |
| Exception | Wird ausgelöst, wenn ein Laufzeitfehler auftritt. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig (zum Beispiel, weil er sich auf einem nicht zugeordneten Laufwerk befindet). |
| IOException | Ein I/O-Fehler ist aufgetreten. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreitet die systemdefinierte maximale Länge. |
| UnauthorizedAccessException | Der Aufrufer hat nicht die erforderliche Berechtigung. -oder- *path* gibt eine schreibgeschützte Datei oder ein Verzeichnis an. |

## Hinweise

Wichtig: Das cpio-Archiv wird in dieser Methode erstellt und anschließend komprimiert, sein Inhalt wird intern gehalten. Achtung bei Speicherverbrauch.

## Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


