---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för lzma-arkiv."
type: docs
weight: 87
url: /sv/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Inställningar för lzma-arkiv.

Lempel–Ziv–Markov-kedjealgoritmen (LZMA) är en algoritm som används för att utföra förlustfri datakomprimering. Denna algoritm använder ett ordboksbaserat komprimeringsschema som är något likt LZ77-algoritmen och har en hög komprimeringsgrad samt en variabel komprimeringsordboksstorlek.

Se mer: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Initierar en ny instans av klassen [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) med standardordboksstorlek, lika med 16 megabyte, antal snabba byte lika med 32 och literal kontextbitar lika med 3. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Hämtar en händelse som utlöses när en del av den råa strömmen komprimeras. |
| [getDictionarySize()](#getDictionarySize--) | Storleken på ordboken (historikbuffert) indikerar hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Hämtar antalet literal kontextbitar. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Hämtar antalet byte som används för snabb matchningssökning i LZMA-algoritmen. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ställer in en händelse som utlöses när en del av den råa strömmen komprimeras. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Storleken på ordboken (historikbuffert) indikerar hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Ställer in antalet literal kontextbitar. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Ställer in antalet byte som används för snabb matchningssökning i LZMA-algoritmen. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Initierar en ny instans av klassen [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) med standardordboksstorlek, lika med 16 megabyte, antal snabba byte lika med 32 och literal kontextbitar lika med 3.

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


Storleken på ordboken (historikbuffert) indikerar hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet. Om den inte är angiven väljs den enligt postens storlek.

Ju större ordboken är, desto bättre är vanligtvis komprimeringsgraden – men ordböcker som är större än den okomprimerade datan är ett slöseri med RAM. Storleken på LZMA-arkivets ordbok måste vara antingen en tvåpotens (2^n) eller tre gånger en tvåpotens (3\*2^n).

**Returns:**
int – Storlek på ordbok (historikbuffert).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Hämtar antalet literal kontextbitar.

Literal kontextbitar definierar hur många av de mest signifikanta bitarna i den föregående okomprimerade byten används för att förutsäga bitarna i nästa literalbyte. Måste vara mellan 0 och 8.

**Returns:**
int – antalet literal kontextbitar.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Hämtar antalet byte som används för snabb matchningssökning i LZMA-algoritmen.

Ett högre värde tillåter komprimeraren att söka längre matchningar, vilket kan förbättra komprimeringsgraden något men sänker komprimeringshastigheten.

**Returns:**
int - antalet byte som används för snabb matchningssökning i LZMA-algoritmen.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Ställer in en händelse som utlöses när en del av den råa strömmen komprimeras.

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

