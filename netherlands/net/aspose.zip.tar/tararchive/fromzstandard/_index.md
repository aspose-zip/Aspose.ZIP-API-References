---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "TarArchive-methode. Extraheert het opgegeven Zstandard-archief en stelt een TarArchive samen uit de geëxtraheerde gegevens"
type: docs
weight: 80
url: /nl/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Extraheert het opgegeven Zstandard-archief en stelt [`TarArchive`](../) samen uit de geëxtraheerde gegevens.

Belangrijk: Zstandard-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bron | Stream | De bron van het archief. |

### Retourwaarde

Een instantie van [`TarArchive`](../)

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| IOException | Zstandard-stroom is beschadigd of niet leesbaar. |
| InvalidDataException | Gegevens zijn beschadigd. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat het verwachte aantal bytes is gelezen. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |

### Zie ook

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Extraheert het opgegeven Zstandard-archief en stelt [`TarArchive`](../) samen uit de geëxtraheerde gegevens.

Belangrijk: Zstandard-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Zstandard-stroom is beschadigd of niet leesbaar. |
| InvalidDataException | Gegevens zijn beschadigd. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat het verwachte aantal bytes is gelezen. |

### Zie ook

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


