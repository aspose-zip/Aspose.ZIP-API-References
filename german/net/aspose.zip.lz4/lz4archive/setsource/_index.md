---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Lz4Archive-Methode. Legt den Inhalt fest, der im Archiv komprimiert werden soll."
type: docs
weight: 70
url: /de/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

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
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

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
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in einen `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tarArchive | TarArchive | Tar-Archiv, das komprimiert werden soll. |
| format | TarFormat | Definiert das Tar-Header-Format. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Dieses Archiv ist für die Extraktion vorbereitet. |

## Hinweise

Verwenden Sie diese Methode, um ein gemeinsames tar.lz4-Archiv zu erstellen.

## Beispiele

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Siehe auch

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

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
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| InvalidOperationException | Dieses Archiv ist für die Extraktion vorbereitet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`.

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


