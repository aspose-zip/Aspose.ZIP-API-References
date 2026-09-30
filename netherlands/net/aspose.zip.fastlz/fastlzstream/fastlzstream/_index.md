---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "FastLZStream constructor. Initialiseert een nieuw exemplaar van de FastLZStream klasse, voorbereid voor compressie"
type: docs
weight: 10
url: /nl/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Initialiseert een nieuw exemplaar van de [`FastLZStream`](../) klasse, voorbereid voor compressie.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stream voor het opslaan van gecomprimeerde gegevens. |
| compressionLevel | Int32 | Gebruik 1 voor snellere compressie, gebruik 2 voor een betere compressieverhouding. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* ondersteunt geen schrijven. |
| ArgumentOutOfRangeException | *compressionLevel* is meer dan 2 of minder dan 1. |

### Zie ook

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


