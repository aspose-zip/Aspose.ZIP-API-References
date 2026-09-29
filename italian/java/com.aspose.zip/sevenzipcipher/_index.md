---
title: "SevenZipCipher"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Classe base per il cifrario AES utilizzato per la crittografia 7-zip."
type: docs
weight: 110
url: /it/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Classe base per il cifrario AES utilizzato per la crittografia 7-zip.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Restituisce un valore che indica se la trasformazione corrente può essere riutilizzata. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Restituisce un valore che indica se più blocchi possono essere trasformati. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [getInputBlockSize()](#getInputBlockSize--) | Restituisce la dimensione del blocco di input. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Restituisce la dimensione del blocco di output. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Trasforma la regione specificata dell'array di byte di input e copia la trasformazione risultante nella regione specificata dell'array di byte di output. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Trasforma la regione specificata dell'array di byte specificato. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Restituisce un valore che indica se la trasformazione corrente può essere riutilizzata.

**Returns:**
boolean - un valore che indica se la trasformazione corrente può essere riutilizzata
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Restituisce un valore che indica se più blocchi possono essere trasformati.

**Returns:**
boolean - un valore che indica se più blocchi possono essere trasformati
### dispose() {#dispose--}
```
public abstract void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Restituisce la dimensione del blocco di input.

**Returns:**
int - la dimensione del blocco di input
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Restituisce la dimensione del blocco di output.

**Returns:**
int - la dimensione del blocco di output
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Trasforma la regione specificata dell'array di byte di input e copia la trasformazione risultante nella regione specificata dell'array di byte di output.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inputBuffer | byte[] | l'input per cui calcolare la trasformazione |
| inputOffset | int | l'offset nell'array di byte di input da cui iniziare a utilizzare i dati |
| inputCount | int | il numero di byte nell'array di byte di input da utilizzare come dati |
| outputBuffer | byte[] | l'output a cui scrivere la trasformazione |
| outputOffset | int | l'offset nell'array di byte di output da cui iniziare a scrivere i dati |

**Returns:**
int - il numero di byte scritti
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Trasforma la regione specificata dell'array di byte specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inputBuffer | byte[] | l'input per cui calcolare la trasformazione |
| inputOffset | int | l'offset nell'array di byte di input da cui iniziare a utilizzare i dati |
| inputCount | int | il numero di byte nell'array di byte di input da utilizzare come dati |

**Returns:**
byte[] - la trasformazione calcolata
