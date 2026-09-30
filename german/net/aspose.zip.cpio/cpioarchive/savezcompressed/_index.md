---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CpioArchive-Methode. Speichert das Archiv in den Stream mit Z-Kompression."
type: docs
weight: 130
url: /de/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Speichert das Archiv in den Stream mit Z-Kompression.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Speichert das Archiv pfadweise mit Z-Kompression.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig (zum Beispiel, weil er sich auf einem nicht zugeordneten Laufwerk befindet). |
| IOException | Ein I/O-Fehler ist aufgetreten. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreitet die systemdefinierte maximale Länge. |

## Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


