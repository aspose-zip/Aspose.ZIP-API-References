---
title: "Klassen FastLZStream"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.FastLZ.FastLZStream-klass. En strömmaskering som komprimerar data med FastLZ. Implementerar dekoratörsmönster"
type: docs
weight: 500
url: /sv/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

En strömomslag som komprimerar data med FastLZ. Implementerar dekoratörsmönster.

```csharp
public class FastLZStream : Stream
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Initierar en ny instans av klassen `FastLZStream` förberedd för komprimering. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Hämtar ett värde som indikerar om den aktuella strömmen stödjer läsning. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Hämtar ett värde som indikerar om den aktuella strömmen stödjer sökning. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Hämtar ett värde som indikerar om den aktuella strömmen stödjer skrivning. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Hämtar strömmens längd i byte. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Hämtar eller anger positionen i den aktuella strömmen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Stänger den aktuella strömmen och frigör eventuella resurser (såsom sockets och filhandtag) som är associerade med den aktuella strömmen. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Rensar alla buffertar för denna ström och får all buffrad data att skrivas till den underliggande enheten. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Läser en sekvens av byte från strömmen och avancerar positionen i strömmen med antalet lästa byte. Stöds inte. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Anger positionen i den aktuella strömmen. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Anger längden på den aktuella strömmen. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Skriver en sekvens av byte till den komprimerande strömmen och avancerar den aktuella positionen i denna ström med antalet skrivna byte. |

### Se även

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


