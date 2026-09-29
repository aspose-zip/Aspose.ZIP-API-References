---
title: "LzmaArchiveSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per l'archivio lzma."
type: docs
weight: 87
url: /it/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Impostazioni per l'archivio lzma.

L'algoritmo Lempel–Ziv–Markov chain (LZMA) è un algoritmo utilizzato per eseguire la compressione dati senza perdita. Questo algoritmo utilizza uno schema di compressione a dizionario leggermente simile all'algoritmo LZ77 e presenta un alto rapporto di compressione e una dimensione del dizionario di compressione variabile.

Vedi di più: [Lempel–Ziv–Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Inizializza una nuova istanza della classe [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) con dimensione del dizionario predefinita, pari a 16 megabyte, numero di byte veloci pari a 32 e bit di contesto letterale pari a 3. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [getDictionarySize()](#getDictionarySize--) | La dimensione del dizionario (buffer di cronologia) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Restituisce il numero di bit di contesto letterale. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Restituisce il numero di byte utilizzati per la ricerca rapida di corrispondenze nell'algoritmo LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | La dimensione del dizionario (buffer di cronologia) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Imposta il numero di bit di contesto letterale. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Imposta il numero di byte utilizzati per la ricerca rapida di corrispondenze nell'algoritmo LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Inizializza una nuova istanza della classe [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) con dimensione del dizionario predefinita, pari a 16 megabyte, numero di byte veloci pari a 32 e bit di contesto letterale pari a 3.

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


La dimensione del dizionario (buffer di cronologia) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria. Se non impostata, verrà scelta in base alla dimensione della voce.

Più grande è il dizionario, di solito migliore è il rapporto di compressione - ma i dizionari più grandi dei dati non compressi sono uno spreco di RAM. La dimensione del dizionario di un archivio LZMA deve essere una potenza di due (2^n) o tre volte una potenza di due (3\*2^n).

**Returns:**
int - Dimensione del dizionario (buffer di cronologia).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Restituisce il numero di bit di contesto letterale.

I bit di contesto letterale definiscono quanti dei bit più significativi del byte non compresso precedente sono utilizzati per prevedere i bit del byte letterale successivo. Devono essere da 0 a 8.

**Returns:**
int - il numero di bit di contesto letterale.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Restituisce il numero di byte utilizzati per la ricerca rapida di corrispondenze nell'algoritmo LZMA.

Un valore più alto consente al compressore di cercare corrispondenze più lunghe, il che può migliorare leggermente il rapporto di compressione ma rallenta la compressione.

**Returns:**
int - il numero di byte usati per la ricerca di corrispondenze rapide nell'algoritmo LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Imposta un evento che viene sollevato quando una porzione di stream grezzo è compressa.

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

