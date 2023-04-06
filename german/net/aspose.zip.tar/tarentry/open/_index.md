---
title: TarEntry.Open
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarEntry methode. Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit.
type: docs
weight: 50
url: /de/net/aspose.zip.tar/tarentry/open/
---
## TarEntry.Open method

Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit.

```csharp
public Stream Open()
```

### Rückgabewert

Der Stream, der den Inhalt des Eintrags darstellt.

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
Stream decompressed = entry.Open();
```

### Siehe auch

* class [TarEntry](../)
* namensraum [Aspose.Zip.Tar](../../tarentry/)
* Montage [Aspose.Zip](../../../)


