---
title: SharArchive.Save
second_title: Aspose.ZIP für .NET-API-Referenz
description: SharArchive methode. Speichert das Archiv in der bereitgestellten Zieldatei.
type: docs
weight: 70
url: /de/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Speichert das Archiv in der bereitgestellten Zieldatei.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destinationFileName* ist eine leere Zeichenfolge, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen gemäß der Definition von System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* ist Null. |
| PathTooLongException | Die angegebene*destinationFileName*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| DirectoryNotFoundException | Die angegebene*destinationFileName* ungültig ist (z. B. auf einem nicht zugeordneten Laufwerk). |
| IOException | Beim Öffnen der Datei ist ein E/A-Fehler aufgetreten. |
| UnauthorizedAccessException | *destinationFileName* eine Datei angegeben, die schreibgeschützt ist und der Zugriff nicht Read ist. – oder – Pfad ein Verzeichnis angegeben. – oder – Der Aufrufer hat nicht die erforderliche Berechtigung. |
| NotSupportedException | *destinationFileName* hat ein ungültiges Format. |

### Bemerkungen

Es ist möglich, ein Archiv unter demselben Pfad zu speichern, aus dem es geladen wurde. Dies wird jedoch nicht empfohlen, da dieser Ansatz das Kopieren in eine temporäre Datei verwendet.

### Beispiele

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Siehe auch

* class [SharArchive](../)
* namensraum [Aspose.Zip.Shar](../../shararchive/)
* Montage [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Speichert das Archiv im bereitgestellten Stream.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| output | Stream | Zielstrom. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist Null. |
| ArgumentException | *output* ist nicht beschreibbar. - oder -*output* ist der gleiche Strom, aus dem wir extrahieren. |

### Bemerkungen

*output*muss beschreibbar sein.

### Beispiele

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Siehe auch

* class [SharArchive](../)
* namensraum [Aspose.Zip.Shar](../../shararchive/)
* Montage [Aspose.Zip](../../../)


