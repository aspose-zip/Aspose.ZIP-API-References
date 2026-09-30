---
title: "UueArchive.Open"
second_title: "Aspose.ZIP för .NET API-referens"
description: "UueArchive-metod. Öppnar arkivet för avkodning och tillhandahåller en ström med arkivinnehåll"
type: docs
weight: 60
url: /sv/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Öppnar arkivet för avkodning och tillhandahåller en ström med arkivinnehåll.

```csharp
public Stream Open()
```

### Returvärde

Strömmen som representerar arkivets innehåll.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Läs från strömmen för att få originalinnehållet i en fil. Se avsnittet exempel.

## Exempel

Användning:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 och högre - använd metoden Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 och tidigare - kopiera byte manuellt:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Se även

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


