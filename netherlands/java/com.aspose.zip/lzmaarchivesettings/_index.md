---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor een lzma-archief."
type: docs
weight: 87
url: /nl/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Instellingen voor een lzma-archief.

Het Lempel\u2013Ziv\u2013Markov chain-algoritme (LZMA) is een algoritme dat wordt gebruikt om verliesloze gegevenscompressie uit te voeren. Dit algoritme gebruikt een woordenboekcompressieschema dat enigszins vergelijkbaar is met het LZ77-algoritme en biedt een hoge compressieverhouding en een variabele compressiewoordenboekgrootte.

Zie meer: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Initialiseert een nieuw exemplaar van de [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) klasse met een standaard woordenboekgrootte van 16 megabyte, een aantal snelle bytes gelijk aan 32 en letterlijke contextbits gelijk aan 3. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [getDictionarySize()](#getDictionarySize--) | De grootte van het woordenboek (geschiedenisbuffer) geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Haalt het aantal letterlijke contextbits op. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Haalt het aantal bytes op dat wordt gebruikt voor snelle overeenkomstzoekopdrachten in het LZMA-algoritme. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | De grootte van het woordenboek (geschiedenisbuffer) geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Stelt het aantal letterlijke contextbits in. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Stelt het aantal bytes in dat wordt gebruikt voor snelle overeenkomstzoekopdrachten in het LZMA-algoritme. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Initialiseert een nieuw exemplaar van de [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) klasse met een standaard woordenboekgrootte van 16 megabyte, een aantal snelle bytes gelijk aan 32 en letterlijke contextbits gelijk aan 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


De grootte van het woordenboek (geschiedenisbuffer) geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. Indien niet ingesteld, wordt deze gekozen op basis van de grootte van de invoer.

Hoe groter het woordenboek, hoe beter de compressieverhouding meestal is – maar woordenboeken die groter zijn dan de ongecomprimeerde gegevens zijn een verspilling van RAM. De woordenboekgrootte van een LZMA-archief moet ofwel een macht van twee (2^n) zijn of drie keer een macht van twee (3\*2^n).

**Returns:**
int - Grootte van het woordenboek (geschiedenisbuffer).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Haalt het aantal letterlijke contextbits op.

Letterlijke contextbits definiëren hoeveel van de meest significante bits van de vorige ongecomprimeerde byte worden gebruikt om de bits van de volgende letterlijke byte te voorspellen. Moet tussen 0 en 8 liggen.

**Returns:**
int - het aantal letterlijke contextbits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Haalt het aantal bytes op dat wordt gebruikt voor snelle overeenkomstzoekopdrachten in het LZMA-algoritme.

Een hogere waarde stelt de compressor in staat om langere overeenkomsten te zoeken, wat de compressieverhouding enigszins kan verbeteren, maar de compressie vertraagt.

**Returns:**
int - het aantal bytes dat wordt gebruikt voor snelle overeenkomstzoekopdrachten in het LZMA-algoritme.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

