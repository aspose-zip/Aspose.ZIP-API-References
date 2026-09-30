---
title: "TarArchive.SaveZstandard"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "TarArchive-Methode. Speichert das Archiv in den Stream mit Zstandard-Kompression"
type: docs
weight: 220
url: /de/net/aspose.zip.tar/tararchive/savezstandard/
---
## SaveZstandard(Stream, TarFormat?) {#savezstandard}

Speichert das Archiv in den Stream mit Zstandard-Kompression.

```csharp
public void SaveZstandard(Stream output, TarFormat? format = default)
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

## Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.tar.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, TarFormat?) {#savezstandard_1}

Speichert das Archiv in die Datei unter dem Pfad mit Zstandard-Kompression.

```csharp
public void SaveZstandard(string path, TarFormat? format = default)
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

## Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.tar.zst");
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


