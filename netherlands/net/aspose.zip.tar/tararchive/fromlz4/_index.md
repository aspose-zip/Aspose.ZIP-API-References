---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "TarArchive-methode. Extraheert opgegeven LZ4-archief en stelt TarArchive samen uit de geëxtraheerde gegevens"
type: docs
weight: 30
url: /nl/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Extraheert opgegeven LZ4-archief en stelt [`TarArchive`](../) samen uit de geëxtraheerde gegevens.

Belangrijk: LZ4-archief wordt volledig geëxtraheerd binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* heeft een ongeldig formaat. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| FileNotFoundException | Het bestand is niet gevonden. |
| EndOfStreamException | Het bestand is te kort. |
| InvalidDataException | Het bestand heeft een onjuiste handtekening. |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |
| InvalidOperationException | Het archief is voorbereid op samenstelling. |

## Opmerkingen

LZ4-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie-algoritme. Tar-archief biedt de mogelijkheid om willekeurige records te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken.

### Zie ook

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Extraheert opgegeven LZ4-archief en stelt [`TarArchive`](../) samen uit de geëxtraheerde gegevens.

Belangrijk: LZ4-archief wordt volledig geëxtraheerd binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bron | Stream | De bron van het archief. |

### Retourwaarde

Een instantie van [`TarArchive`](../)

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | Kan niet lezen van *source* |
| ArgumentNullException | *source* is null. |
| EndOfStreamException | *source* is te kort. |
| InvalidDataException | De *source* heeft een onjuiste handtekening. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |

## Opmerkingen

LZ4-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie-algoritme. Tar-archief biedt de mogelijkheid om willekeurige records te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken.

### Zie ook

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


