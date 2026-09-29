---
title: "FastLZOutputStream"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Un wrapper di stream che comprime i dati con FastLZ."
type: docs
weight: 68
url: /it/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Un wrapper di stream che comprime i dati con FastLZ. Implementa il pattern decoratore.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Inizializza una nuova istanza della classe FastLZStream preparata per la compressione. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | Chiude lo stream corrente e rilascia tutte le risorse (come socket e handle di file) associate allo stream corrente. |
| [flush()](#flush--) | Svuota tutti i buffer per questo stream e fa sì che i dati memorizzati vengano scritti sul dispositivo sottostante. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Scrive una sequenza di byte nello stream di compressione e avanza la posizione corrente all'interno di questo stream del numero di byte scritti. |
| [write(int b)](#write-int-) | Scrive il byte specificato in questo stream di output. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Inizializza una nuova istanza della classe FastLZStream preparata per la compressione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | lo stream per salvare i dati compressi |
| compressionLevel | int | usa 1 per una compressione più veloce, usa 2 per un rapporto di compressione migliore |

### close() {#close--}
```
public void close()
```


Chiude lo stream corrente e rilascia tutte le risorse (come socket e handle di file) associate allo stream corrente.

### flush() {#flush--}
```
public void flush()
```


Svuota tutti i buffer per questo stream e fa sì che i dati memorizzati vengano scritti sul dispositivo sottostante.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Scrive una sequenza di byte nello stream di compressione e avanza la posizione corrente all'interno di questo stream del numero di byte scritti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| buffer | byte[] | un array di byte. Questo metodo copia count byte dal buffer allo stream corrente |
| offset | int | l'offset di byte basato su zero nel buffer da cui iniziare a copiare i byte nello stream corrente |
| count | int | il numero di byte da scrivere nello stream corrente |

### write(int b) {#write-int-}
```
public void write(int b)
```


Scrive il byte specificato in questo stream di output. Il contratto generale per `write` è che un byte venga scritto nello stream di output. Il byte da scrivere sono gli otto bit di ordine inferiore dell'argomento `b`. I 24 bit di ordine superiore di `b` sono ignorati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| b | int | il `byte` |

