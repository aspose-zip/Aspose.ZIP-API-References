---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP för .NET API-referens
description: ParallelOptions fast egendom. Hämtar eller ställer in minnesuppskattning i megabyte tillgängligt för att ta emot komprimerade poster utan att byta till disk. Detta värde är bara vettigt omParallelCompressInMemory inställningen är inneAuto läge.
type: docs
weight: 20
url: /sv/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Hämtar eller ställer in minnesuppskattning i megabyte tillgängligt för att ta emot komprimerade poster utan att byta till disk. Detta värde är bara vettigt om[`ParallelCompressInMemory`](../parallelcompressinmemory/) inställningen är inneAuto läge.

```csharp
public int AvailableMemorySize { get; set; }
```

### Anmärkningar

Detta värde används för att beräkna den största storleken på posten som kan komprimeras parallellt med andra. Alla poster över det beräknade tröskelvärdet kommer att komprimeras sekventiellt. Det är säkert att ha`AvailableMemorySize` egendom lika stor som gratis RAM och ännu större. Som standard antas det att du har minst 200 MB per CPU-kärna.

### Se även

* class [ParallelOptions](../)
* namnutrymme [Aspose.Zip.Saving](../../paralleloptions/)
* hopsättning [Aspose.Zip](../../../)


