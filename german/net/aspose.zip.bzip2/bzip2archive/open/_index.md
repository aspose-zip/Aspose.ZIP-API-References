---
title: Bzip2Archive.Open
second_title: Aspose.ZIP für .NET-API-Referenz
description: Bzip2Archive methode. Öffnet das Archiv zum Extrahieren und stellt einen Stream mit Archivinhalten bereit.
type: docs
weight: 40
url: /de/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Öffnet das Archiv zum Extrahieren und stellt einen Stream mit Archivinhalten bereit.

```csharp
public Stream Open()
```

### Rückgabewert

Der Stream, der den Inhalt des Archivs darstellt.

### Bemerkungen

Aus dem Stream lesen, um den ursprünglichen Inhalt der Datei zu erhalten. Siehe Beispielabschnitt.

### Beispiele

Nutzung:

.NET 4.0 und höher – Stream.CopyTo-Methode verwenden:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 und früher - Bytes manuell kopieren:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = archive.Open();
```

### Siehe auch

* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)


