---
title: "Klasse FastLZStream"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.FastLZ.FastLZStream klasse. Een stream-wrapper die gegevens comprimeert met FastLZ. Implementeert het decorator-patroon."
type: docs
weight: 500
url: /nl/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

Een streamwrapper die gegevens comprimeert met FastLZ. Implementeert het decorator‑patroon.

```csharp
public class FastLZStream : Stream
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Initialiseert een nieuw exemplaar van de `FastLZStream`-klasse, voorbereid voor compressie. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Haalt een waarde op die aangeeft of de huidige stream lezen ondersteunt. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Haalt een waarde op die aangeeft of de huidige stream zoeken ondersteunt. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Haalt een waarde op die aangeeft of de huidige stream schrijven ondersteunt. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Haalt de lengte in bytes van de stream op. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Haalt de positie binnen de huidige stream op of stelt deze in. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Sluit de huidige stream en geeft alle bronnen (zoals sockets en bestandshandles) die aan de huidige stream zijn gekoppeld vrij. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Leegt alle buffers voor deze stream en zorgt ervoor dat alle gebufferde gegevens naar het onderliggende apparaat worden geschreven. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Leest een reeks bytes uit de stream en schuift de positie binnen de stream vooruit met het aantal gelezen bytes. Niet ondersteund. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Stelt de positie binnen de huidige stream in. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Stelt de lengte van de huidige stream in. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Schrijft een reeks bytes naar de comprimerende stream en schuift de huidige positie binnen deze stream vooruit met het aantal geschreven bytes. |

### Zie ook

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


