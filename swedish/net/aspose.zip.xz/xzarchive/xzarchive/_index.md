---
title: XzArchive.XzArchive
second_title: Aspose.ZIP för .NET API-referens
description: XzArchive byggare. Initierar en ny instans avXzArchive klass och komponerar arkivet i xzformat.
type: docs
weight: 10
url: /sv/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Initierar en ny instans av[`XzArchive`](../) klass och komponerar arkivet i xz-format.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | XzArchiveSettings | Uppsättning av inställningsspecifika xz-arkiv: ordbokstorlek, blockstorlek, kontrolltyp. |

### Se även

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Initierar en ny instans av[`XzArchive`](../) klass förberedd för dekomprimering.

```csharp
public XzArchive(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | Stream | Källan till arkivet. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *source* är inte sökbar. |
| ArgumentNullException | *source* är inget. |

### Anmärkningar

Denna konstruktor dekomprimerar inte. Ser[`Extract`](../extract/) metod för dekomprimering.

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Initierar en ny instans av[`XzArchive`](../) klass förberedd för dekomprimering.

```csharp
public XzArchive(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökväg till källan till arkivet. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Anmärkningar

Denna konstruktor dekomprimerar inte. Ser[`Extract`](../extract/) metod för dekomprimering.

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)


