---
title: "TarArchive.FromLZMA"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "TarArchive-methode. Extraheert het opgegeven LZMA-archief en stelt een TarArchive samen uit de geëxtraheerde gegevens"
type: docs
weight: 50
url: /nl/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Extraheert het opgegeven LZMA-archief en stelt [`TarArchive`](../) samen uit de geëxtraheerde gegevens.

Belangrijk: LZMA-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bron | Stream | De bron van het archief. |

### Retourwaarde

Een instantie van [`TarArchive`](../)

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidDataException | Het archief is beschadigd. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat het verwachte aantal bytes is gelezen. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| ArgumentNullException | *source* is null. |
| IOException | Er treedt een I/O-fout op. |

## Opmerkingen

LZMA-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie-algoritme. Een tar-archief biedt de mogelijkheid om willekeurige records te extraheren, dus moet het onder de motorkap met een doorzoekbare stroom werken.

### Zie ook

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Extraheert het opgegeven LZMA-archief en stelt [`TarArchive`](../) samen uit de geëxtraheerde gegevens.

Belangrijk: LZMA-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

```csharp
public static TarArchive FromLZMA(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het archiefbestand. |

### Retourwaarde

Een instantie van [`TarArchive`](../)

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* heeft een ongeldig formaat. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| FileNotFoundException | Het bestand is niet gevonden. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat het verwachte aantal bytes is gelezen. |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |
| InvalidDataException | Het archief is beschadigd. |

## Opmerkingen

LZMA-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie-algoritme. Een tar-archief biedt de mogelijkheid om willekeurige records te extraheren, dus moet het onder de motorkap met een doorzoekbare stroom werken.

### Zie ook

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


