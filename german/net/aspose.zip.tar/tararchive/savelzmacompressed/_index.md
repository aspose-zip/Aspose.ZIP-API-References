---
title: "TarArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "TarArchive-Methode. Speichert das Archiv in den Stream mit LZMA-Kompression."
type: docs
weight: 190
url: /de/net/aspose.zip.tar/tararchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, TarFormat?) {#savelzmacompressed}

Speichert das Archiv in den Stream mit LZMA-Kompression.

```csharp
public void SaveLZMACompressed(Stream output, TarFormat? format = default)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | Stream | Ziel-Stream. |
| format | Nullable`1 | Definiert das TAR-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist null. |
| ArgumentException | *output* ist nicht beschreibbar. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Hinweise

*output* must be writable.

Wichtig: Das Tar-Archiv wird in dieser Methode erstellt und anschließend komprimiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

## Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.tar.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, TarFormat?) {#savelzmacompressed_1}

Speichert das Archiv in die Datei über den Pfad mit lzma-Kompression.

```csharp
public void SaveLZMACompressed(string path, TarFormat? format = default)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| format | Nullable`1 | Definiert das TAR-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| UnauthorizedAccessException | Der Aufrufer hat nicht die erforderliche Berechtigung. -oder- *path* gibt eine schreibgeschützte Datei oder ein Verzeichnis an. |
| ArgumentException | *path* ist eine Zeichenkette mit Länge null, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen, wie durch InvalidPathChars definiert. |
| ArgumentNullException | *path* ist null. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| DirectoryNotFoundException | Der angegebene *path* ist ungültig (zum Beispiel befindet er sich auf einem nicht zugeordneten Laufwerk). |
| NotSupportedException | *path* hat ein ungültiges Format. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Hinweise

Wichtig: Das Tar-Archiv wird in dieser Methode erstellt und anschließend komprimiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

## Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.tar.lzma");
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


