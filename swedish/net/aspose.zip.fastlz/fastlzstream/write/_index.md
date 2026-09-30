---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP för .NET API-referens"
description: "FastLZStream metod. Skriver en sekvens av byte till den komprimerande strömmen och avancerar den aktuella positionen i denna ström med antalet skrivna byte."
type: docs
weight: 120
url: /sv/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Skriver en sekvens av byte till den komprimerande strömmen och avancerar den aktuella positionen i denna ström med antalet skrivna byte.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| buffert | Byte[] | En array av byte. Denna metod kopierar count byte från buffert till den aktuella strömmen. |
| förskjutning | Int32 | Det nollbaserade byteoffsetet i buffert där kopieringen av byte till den aktuella strömmen ska börja. |
| count | Int32 | Antalet byte som ska skrivas till den aktuella strömmen. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Kastas om strömmen har aviserats. |
| ArgumentNullException | *buffer* är `null`. |

### Se även

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


