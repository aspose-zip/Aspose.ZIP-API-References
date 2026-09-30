---
title: "ZstandardArchive.SetSource"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardArchive-Methode. Legt den Inhalt fest, der im Archiv komprimiert werden soll."
type: docs
weight: 70
url: /de/net/aspose.zip.zstandard/zstandardarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```csharp
public void SetSource(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quelle | Stream | Der Eingabestream für das Archiv. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (var archive = new ZstandardArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.zst");
}
```

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | FileInfo | Der Verweis auf eine zu komprimierende Datei. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.zst");
}
```

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```csharp
public void SetSource(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Pfad zur zu komprimierenden Datei. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |

## Beispiele

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


