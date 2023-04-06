---
title: XzArchive.XzArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: XzArchive constructeur. Initialiseert een nieuw exemplaar van hetXzArchive class en stelt het archief samen in xzindeling.
type: docs
weight: 10
url: /nl/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Initialiseert een nieuw exemplaar van het[`XzArchive`](../) class en stelt het archief samen in xz-indeling.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | XzArchiveSettings | Set instellingen specifiek xz-archief: woordenboekgrootte, blokgrootte, controletype. |

### Zie ook

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* naamruimte [Aspose.Zip.Xz](../../xzarchive/)
* montage [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`XzArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public XzArchive(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | Stream | De bron van het archief. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *source* is niet zoek. |
| ArgumentNullException | *source* is niets. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Extract`](../extract/) methode voor decomprimeren.

### Zie ook

* class [XzArchive](../)
* naamruimte [Aspose.Zip.Xz](../../xzarchive/)
* montage [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`XzArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public XzArchive(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Pad naar de bron van het archief. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Extract`](../extract/) methode voor decomprimeren.

### Zie ook

* class [XzArchive](../)
* naamruimte [Aspose.Zip.Xz](../../xzarchive/)
* montage [Aspose.Zip](../../../)


