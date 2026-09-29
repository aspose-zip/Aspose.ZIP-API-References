---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Een streamwrapper die gegevens comprimeert met FastLZ."
type: docs
weight: 68
url: /nl/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Een streamwrapper die gegevens comprimeert met FastLZ. Implementeert het decorator‑patroon.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Initialiseert een nieuw exemplaar van de FastLZStream‑klasse, voorbereid op compressie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | Sluit de huidige stream en geeft alle bronnen (zoals sockets en bestands‑handles) die aan de huidige stream zijn gekoppeld vrij. |
| [flush()](#flush--) | Leegt alle buffers voor deze stream en zorgt ervoor dat alle gebufferde gegevens naar het onderliggende apparaat worden geschreven. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Schrijft een reeks bytes naar de comprimerende stream en verplaatst de huidige positie binnen deze stream met het aantal geschreven bytes. |
| [write(int b)](#write-int-) | Schrijft het opgegeven byte naar deze output‑stream. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Initialiseert een nieuw exemplaar van de FastLZStream‑klasse, voorbereid op compressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.OutputStream | de stream voor het opslaan van gecomprimeerde gegevens |
| compressionLevel | int | gebruik 1 voor snellere compressie, gebruik 2 voor een betere compressieverhouding |

### close() {#close--}
```
public void close()
```


Sluit de huidige stream en geeft alle bronnen (zoals sockets en bestands‑handles) die aan de huidige stream zijn gekoppeld vrij.

### flush() {#flush--}
```
public void flush()
```


Leegt alle buffers voor deze stream en zorgt ervoor dat alle gebufferde gegevens naar het onderliggende apparaat worden geschreven.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Schrijft een reeks bytes naar de comprimerende stream en verplaatst de huidige positie binnen deze stream met het aantal geschreven bytes.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| buffer | byte[] | een array van bytes. Deze methode kopieert count bytes van buffer naar de huidige stream |
| offset | int | de nulgebaseerde byte‑offset in buffer waar het kopiëren van bytes naar de huidige stream moet beginnen |
| count | int | het aantal bytes dat naar de huidige stream moet worden geschreven |

### write(int b) {#write-int-}
```
public void write(int b)
```


Schrijft het opgegeven byte naar deze output‑stream. Het algemene contract voor `write` is dat één byte naar de output‑stream wordt geschreven. Het te schrijven byte is de acht laagste bits van het argument `b`. De 24 hoogste bits van `b` worden genegeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| b | int | de `byte` |

