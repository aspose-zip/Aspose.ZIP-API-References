---
title: "CpioArchive.SaveLzipped"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CpioArchive-Methode. Speichert das Archiv mit lzip-Kompression im Stream"
type: docs
weight: 100
url: /de/net/aspose.zip.cpio/cpioarchive/savelzipped/
---
## SaveLzipped(Stream, CpioFormat) {#savelzipped}

Speichert das Archiv mit lzip-Kompression im Stream.

```csharp
public void SaveLzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | Stream | Ziel-Stream. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist null. |
| ArgumentException | *output* ist nicht beschreibbar. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

*output* must be writable.

## Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
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

## SaveLzipped(string, CpioFormat) {#savelzipped_1}

Speichert das Archiv über den Pfad mit lzip-Kompression in einer Datei.

```csharp
public void SaveLzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentException | *path* ist eine Zeichenkette mit Länge null, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen, wie durch InvalidPathChars definiert. |
| ArgumentNullException | *path* ist `null`. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig (zum Beispiel, weil er sich auf einem nicht zugeordneten Laufwerk befindet). |
| IOException | Ein I/O-Fehler ist aufgetreten. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreitet die systemdefinierte maximale Länge. |
| UnauthorizedAccessException | Der Aufrufer hat nicht die erforderliche Berechtigung. -oder- *path* gibt eine schreibgeschützte Datei oder ein Verzeichnis an. |

## Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.lz");
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


