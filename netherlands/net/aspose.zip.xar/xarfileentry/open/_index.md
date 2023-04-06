---
title: XarFileEntry.Open
second_title: Aspose.ZIP voor .NET API-referentie
description: XarFileEntry methode. Opent het item voor extractie en biedt een stream met inhoud van het item.
type: docs
weight: 30
url: /nl/net/aspose.zip.xar/xarfileentry/open/
---
## XarFileEntry.Open method

Opent het item voor extractie en biedt een stream met inhoud van het item.

```csharp
public abstract Stream Open()
```

### Winstwaarde

De stream die de inhoud van het item vertegenwoordigt.

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
Stream decompressed = entry.Open();
```

### Zie ook

* class [XarFileEntry](../)
* naamruimte [Aspose.Zip.Xar](../../xarfileentry/)
* montage [Aspose.Zip](../../../)


