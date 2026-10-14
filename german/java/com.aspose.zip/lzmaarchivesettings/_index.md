---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für das LZMA-Archiv."
type: docs
weight: 87
url: /de/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Einstellungen für das LZMA-Archiv.

Der Lempel\u2013Ziv\u2013Markov‑Ketten‑Algorithmus (LZMA) ist ein Algorithmus, der zur verlustfreien Datenkompression verwendet wird. Dieser Algorithmus verwendet ein Wörterbuchkompressionsverfahren, das dem LZ77-Algorithmus etwas ähnlich ist, und bietet ein hohes Kompressionsverhältnis sowie eine variable Größe des Kompressionswörterbuchs.

Siehe mehr: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Initialisiert eine neue Instanz der [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings)-Klasse mit der Standard‑Wörterbuchgröße von 16 Megabyte, einer Anzahl schneller Bytes von 32 und Literal‑Kontext‑Bits von 3. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [getDictionarySize()](#getDictionarySize--) | Die Größe des Wörterbuchs (History‑Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Liefert die Anzahl der Literal‑Kontext‑Bits. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Liefert die Anzahl der Bytes, die für die schnelle Mustersuche im LZMA‑Algorithmus verwendet werden. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Die Größe des Wörterbuchs (History‑Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Setzt die Anzahl der Literal‑Kontext‑Bits. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Setzt die Anzahl der Bytes, die für die schnelle Mustersuche im LZMA‑Algorithmus verwendet werden. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Initialisiert eine neue Instanz der [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings)-Klasse mit der Standard‑Wörterbuchgröße von 16 Megabyte, einer Anzahl schneller Bytes von 32 und Literal‑Kontext‑Bits von 3.

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


Die Größe des Wörterbuchs (History‑Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. Wenn nicht festgelegt, wird sie entsprechend der Eintragsgröße gewählt.

Je größer das Wörterbuch, desto besser ist in der Regel das Kompressionsverhältnis – aber Wörterbücher, die größer als die unkomprimierten Daten sind, verschwenden RAM. Die Wörterbuchgröße eines LZMA‑Archivs muss entweder eine Potenz von zwei (2^n) oder das Dreifache einer Potenz von zwei (3\*2^n) sein.

**Returns:**
int – Wörterbuchgröße (History‑Puffer).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Liefert die Anzahl der Literal‑Kontext‑Bits.

Literal‑Kontext‑Bits definieren, wie viele der höchstwertigen Bits des vorherigen unkomprimierten Bytes verwendet werden, um die Bits des nächsten Literal‑Bytes vorherzusagen. Wertebereich: 0 bis 8.

**Returns:**
int – die Anzahl der Literal‑Kontext‑Bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Liefert die Anzahl der Bytes, die für die schnelle Mustersuche im LZMA‑Algorithmus verwendet werden.

Ein höherer Wert ermöglicht dem Kompressor, längere Übereinstimmungen zu suchen, was das Kompressionsverhältnis leicht verbessern kann, aber die Kompression verlangsamt.

**Returns:**
int – die Anzahl der Bytes, die für die schnelle Übereinstimmungssuche im LZMA-Algorithmus verwendet werden.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird.

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

