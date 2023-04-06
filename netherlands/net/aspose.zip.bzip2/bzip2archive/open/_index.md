---
title: Bzip2Archive.Open
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2Archive methode. Opent het archief voor extractie en levert een stream met archiefinhoud.
type: docs
weight: 40
url: /nl/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Opent het archief voor extractie en levert een stream met archiefinhoud.

```csharp
public Stream Open()
```

### Winstwaarde

De stream die de inhoud van het archief vertegenwoordigt.

### Opmerkingen

Lees uit de stream om de originele inhoud van het bestand te krijgen. Zie voorbeelden sectie.

### Voorbeelden

Gebruik:

.NET 4.0 en hoger - gebruik de Stream.CopyTo-methode:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 en eerder - bytes handmatig kopiëren:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = archive.Open();
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)


