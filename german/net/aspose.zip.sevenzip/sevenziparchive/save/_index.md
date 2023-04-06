---
title: SevenZipArchive.Save
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipArchive methode. Speichert das 7zArchiv im bereitgestellten Stream.
type: docs
weight: 80
url: /de/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Speichert das 7z-Archiv im bereitgestellten Stream.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| output | Stream | Zielstrom. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *output* unterstützt nicht das Suchen. |
| ArgumentNullException | *output* ist Null. |
| InvalidOperationException | Encoder konnte Daten nicht komprimieren. |

### Bemerkungen

*output* muss auffindbar sein.

### Beispiele

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Siehe auch

* class [SevenZipArchive](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Montage [Aspose.Zip](../../../)

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
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Siehe auch

* class [SevenZipArchive](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Montage [Aspose.Zip](../../../)


