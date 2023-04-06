---
title: SevenZipArchiveEntry.Open
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipArchiveEntry methode. Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit.
type: docs
weight: 90
url: /de/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit.

```csharp
public Stream Open(string password = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | String | Optionales Passwort für die Entschlüsselung. |

### Rückgabewert

Der Stream, der den Inhalt des Eintrags darstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Das Archiv wird nicht zum Entpacken geöffnet. - oder - Dieser Eintrag ist ein Verzeichnis. |
| InvalidDataException | Falsche Daten im Eintrag. |

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

* class [SevenZipArchiveEntry](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Montage [Aspose.Zip](../../../)


