---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AppleArchive-methode. Slaat het archief op in de opgegeven stroom."
type: docs
weight: 90
url: /nl/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Slaat het archief op in de opgegeven stream.

```csharp
public void Save(Stream output)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uitvoer | Stream | Doelstream. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Het archief is vrijgegeven. |
| ArgumentNullException | *output* is `null`. |
| ArgumentException | *output* is niet beschrijfbaar. |
| ArgumentOutOfRangeException | Geconfigureerde LZ4- of Zlib-blokgrootte is niet positief. |
| NotSupportedException | Compressie-instellingen ontbreken of worden niet ondersteund, directe compositie gebruikt een niet-zoekbare stroom, of de grootte van de vermelding/het archief overschrijdt de huidige limieten van Apple Archive. |

## Opmerkingen

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Zie ook

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Slaat het archief op in een opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het te creëren archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Het archief is vrijgegeven. |
| ArgumentException | *destinationFileName* is ongeldig. |
| ArgumentNullException | *destinationFileName* is `null`. |
| ArgumentOutOfRangeException | Geconfigureerde LZ4- of Zlib-blokgrootte is niet positief. |
| NotSupportedException | Compressie-instellingen ontbreken of worden niet ondersteund, directe compositie gebruikt een niet-zoekbare stroom, of de grootte van de vermelding/het archief overschrijdt de huidige limieten van Apple Archive. |

### Zie ook

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


