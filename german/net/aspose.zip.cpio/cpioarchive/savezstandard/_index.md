---
title: "CpioArchive.SaveZstandard"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CpioArchive-Methode. Speichert das Archiv in den Stream mit Zstandard-Kompression."
type: docs
weight: 140
url: /de/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Speichert das Archiv in den Stream mit Zstandard-Kompression.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Speichert das Archiv in die Datei unter dem Pfad mit Zstandard-Kompression.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


