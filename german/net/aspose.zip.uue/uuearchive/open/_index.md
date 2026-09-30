---
title: "UueArchive.Open"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "UueArchive-Methode. Öffnet das Archiv zum Dekodieren und liefert einen Stream mit dem Archivinhalt"
type: docs
weight: 60
url: /de/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Öffnet das Archiv zum Dekodieren und liefert einen Stream mit dem Archivinhalt.

```csharp
public Stream Open()
```

### Rückgabewert

Der Stream, der den Inhalt des Archivs darstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Lesen Sie aus dem Stream, um den ursprünglichen Inhalt einer Datei zu erhalten. Siehe den Abschnitt Beispiele.

## Beispiele

Verwendung:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 und höher – verwenden Sie die Methode Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 und früher – Bytes manuell kopieren:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Siehe auch

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


