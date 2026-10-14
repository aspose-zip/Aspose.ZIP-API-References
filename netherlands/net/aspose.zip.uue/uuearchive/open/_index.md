---
title: "UueArchive.Open"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "UueArchive-methode. Opent het archief voor decodering en levert een stream met de archiefinhoud"
type: docs
weight: 60
url: /nl/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Opent het archief voor decodering en levert een stream met de archiefinhoud.

```csharp
public Stream Open()
```

### Retourwaarde

De stream die de inhoud van het archief vertegenwoordigt.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

Lees van de stream om de oorspronkelijke inhoud van een bestand te verkrijgen. Zie de sectie voorbeelden.

## Voorbeelden

Gebruik:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 en hoger - gebruik de Stream.CopyTo-methode:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 en eerder - kopieer bytes handmatig:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Zie ook

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


