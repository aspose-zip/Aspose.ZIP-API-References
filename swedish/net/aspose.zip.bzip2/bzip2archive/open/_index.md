---
title: Bzip2Archive.Open
second_title: Aspose.ZIP för .NET API-referens
description: Bzip2Archive metod. Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehåll.
type: docs
weight: 40
url: /sv/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehåll.

```csharp
public Stream Open()
```

### Returvärde

Strömmen som representerar innehållet i arkivet.

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
Stream decompressed = archive.Open();
```

### Se även

* class [Bzip2Archive](../)
* namnutrymme [Aspose.Zip.Bzip2](../../bzip2archive/)
* hopsättning [Aspose.Zip](../../../)


