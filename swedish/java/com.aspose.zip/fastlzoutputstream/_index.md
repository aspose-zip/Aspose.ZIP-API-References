---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP för Java API-referens"
description: "En strömwrapper som komprimerar data med FastLZ."
type: docs
weight: 68
url: /sv/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

En strömomslag som komprimerar data med FastLZ. Implementerar dekoratörsmönster.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Initierar en ny instans av FastLZStream-klassen förberedd för kompression. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | Stänger den aktuella strömmen och frigör eventuella resurser (såsom sockets och filhandtag) som är associerade med den aktuella strömmen. |
| [flush()](#flush--) | Rensar alla buffertar för denna ström och får all buffrad data att skrivas till den underliggande enheten. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Skriver en sekvens av byte till den komprimerande strömmen och förflyttar den aktuella positionen i denna ström med antalet skrivna byte. |
| [write(int b)](#write-int-) | Skriver den angivna byte till denna utdataström. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Initierar en ny instans av FastLZStream-klassen förberedd för kompression.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | strömmen för att spara komprimerad data |
| compressionLevel | int | använd 1 för snabbare kompression, använd 2 för bättre komprimeringsförhållande |

### close() {#close--}
```
public void close()
```


Stänger den aktuella strömmen och frigör eventuella resurser (såsom sockets och filhandtag) som är associerade med den aktuella strömmen.

### flush() {#flush--}
```
public void flush()
```


Rensar alla buffertar för denna ström och får all buffrad data att skrivas till den underliggande enheten.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Skriver en sekvens av byte till den komprimerande strömmen och förflyttar den aktuella positionen i denna ström med antalet skrivna byte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| buffert | byte[] | en array av byte. Denna metod kopierar count byte från bufferten till den aktuella strömmen |
| offset | int | det nollbaserade byteoffsetet i bufferten där kopieringen av byte till den aktuella strömmen ska börja |
| count | int | antalet byte som ska skrivas till den aktuella strömmen |

### write(int b) {#write-int-}
```
public void write(int b)
```


Skriver den angivna byte till denna utdataström. Det allmänna kontraktet för `write` är att en byte skrivs till utdataströmmen. Byten som ska skrivas är de åtta lägsta bitarna i argumentet `b`. De 24 högsta bitarna i `b` ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| b | int | det `byte` |

