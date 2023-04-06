---
title: ZArchive.ZArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: ZArchive constructeur. Initialiseert een nieuw exemplaar van hetZArchive klasse voorbereid voor compressie.
type: docs
weight: 10
url: /nl/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Initialiseert een nieuw exemplaar van het[`ZArchive`](../) klasse voorbereid voor compressie.

```csharp
public ZArchive()
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`ZArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public ZArchive(Stream source)
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

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`ZArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public ZArchive(string path)
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

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)


