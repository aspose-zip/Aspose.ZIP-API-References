---
title: ArchiveEntry.Open
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveEntry metod. Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll.
type: docs
weight: 110
url: /sv/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll.

```csharp
public Stream Open(string password = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| password | String | Valfritt lösenord för dekryptering. |

### Returvärde

Strömmen som representerar innehållet i posten.

### Anmärkningar

Läs från strömmen för att få originalinnehållet i filen. Se avsnittet med exempel.

### Exempel

Användning:

.NET 4.0 och senare - använd Stream.CopyTo-metoden:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 och tidigare - kopiera bytes manuellt:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Se även

* class [ArchiveEntry](../)
* namnutrymme [Aspose.Zip](../../archiveentry/)
* hopsättning [Aspose.Zip](../../../)


