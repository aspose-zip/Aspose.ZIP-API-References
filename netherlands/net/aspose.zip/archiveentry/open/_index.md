---
title: ArchiveEntry.Open
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveEntry methode. Opent het item voor extractie en biedt een stream met gedecomprimeerde inhoud van het item.
type: docs
weight: 110
url: /nl/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Opent het item voor extractie en biedt een stream met gedecomprimeerde inhoud van het item.

```csharp
public Stream Open(string password = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | String | Optioneel wachtwoord voor decodering. |

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

* class [ArchiveEntry](../)
* naamruimte [Aspose.Zip](../../archiveentry/)
* montage [Aspose.Zip](../../../)


