---
title: "SevenZipCipher"
second_title: "Aspose.ZIP för Java API-referens"
description: "Bas-klass för AES-chiffer som används för 7-zip-kryptering."
type: docs
weight: 110
url: /sv/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Bas-klass för AES-chiffer som används för 7-zip-kryptering.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Hämtar ett värde som indikerar om den aktuella transformationen kan återanvändas. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Hämtar ett värde som indikerar om flera block kan transformeras. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [getInputBlockSize()](#getInputBlockSize--) | Hämtar ingångsblockets storlek. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Hämtar utgångsblockets storlek. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Transformerar det angivna området i inmatningsbytearrayen och kopierar den resulterande transformationen till det angivna området i utmatningsbytearrayen. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Transformerar det angivna området i den angivna bytearrayen. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Hämtar ett värde som indikerar om den aktuella transformationen kan återanvändas.

**Returns:**
boolean - ett värde som indikerar om den aktuella transformationen kan återanvändas
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Hämtar ett värde som indikerar om flera block kan transformeras.

**Returns:**
boolean - ett värde som indikerar om flera block kan transformeras
### dispose() {#dispose--}
```
public abstract void dispose()
```


Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Hämtar ingångsblockets storlek.

**Returns:**
int - ingångsblockets storlek
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Hämtar utgångsblockets storlek.

**Returns:**
int - utgångsblockets storlek
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Transformerar det angivna området i inmatningsbytearrayen och kopierar den resulterande transformationen till det angivna området i utmatningsbytearrayen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inputBuffer | byte[] | indatan för vilken transformationen ska beräknas |
| inputOffset | int | offseten i inmatningsbytearrayen från vilken man börjar använda data |
| inputCount | int | antalet byte i inmatningsbytearrayen som ska användas som data |
| outputBuffer | byte[] | utdata som transformen ska skrivas till |
| outputOffset | int | offseten i utdata-bytearrayen från vilken man börjar skriva data |

**Returns:**
int - antalet skrivna byte
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Transformerar det angivna området i den angivna bytearrayen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inputBuffer | byte[] | indatan för vilken transformationen ska beräknas |
| inputOffset | int | offseten i inmatningsbytearrayen från vilken man börjar använda data |
| inputCount | int | antalet byte i inmatningsbytearrayen som ska användas som data |

**Returns:**
byte[] - den beräknade transformen
