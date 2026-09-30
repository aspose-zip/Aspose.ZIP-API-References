---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Lz4Archive-Methode. Extrahiert das Archiv in die Datei anhand des Pfads"
type: docs
weight: 30
url: /de/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Extrahiert das Archiv in die Datei über den Pfad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

### Rückgabewert

Informationen einer extrahierten Datei.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| EndOfStreamException | Quellstream ist zu kurz. |
| InvalidDataException | Falsche Bytes beim Dekodieren gefunden. |
| NotSupportedException | Diese LZ4-Version wird nicht unterstützt. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Das Archiv ist für die Zusammensetzung vorbereitet. |

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrahiert das Archiv in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |
| EndOfStreamException | Quellstream ist zu kurz. |
| InvalidDataException | Falsche Bytes beim Dekodieren gefunden. |
| NotSupportedException | Diese LZ4-Version wird nicht unterstützt. |
| InvalidOperationException | Das Archiv ist für die Zusammensetzung vorbereitet. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


