---
title: ZArchive.Save
second_title: Aspose.ZIP für .NET-API-Referenz
description: ZArchive methode. Speichert das xzArchiv im bereitgestellten Stream.
type: docs
weight: 40
url: /de/net/aspose.zip.z/zarchive/save/
---
## Save(Stream) {#save}

Speichert das xz-Archiv im bereitgestellten Stream.

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

### Bemerkungen

*output* muss auffindbar sein.

### Beispiele

```csharp
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### Siehe auch

* class [ZArchive](../)
* namensraum [Aspose.Zip.Z](../../zarchive/)
* Montage [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Speichert das Z-Archiv in der bereitgestellten Zieldatei.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | +Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*destinationFileName* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*destinationFileName* ist abgelehnt. |
| PathTooLongException | Die angegebene*destinationFileName*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Beispiele

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Siehe auch

* class [ZArchive](../)
* namensraum [Aspose.Zip.Z](../../zarchive/)
* Montage [Aspose.Zip](../../../)


