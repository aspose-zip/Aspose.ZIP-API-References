---
title: "SevenZipCipher"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Basisklasse voor AES-cijfer gebruikt voor 7-zip-encryptie."
type: docs
weight: 110
url: /nl/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Basisklasse voor AES-cijfer gebruikt voor 7-zip-encryptie.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Haalt een waarde op die aangeeft of de huidige transformatie kan worden hergebruikt. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Haalt een waarde op die aangeeft of meerdere blokken kunnen worden getransformeerd. |
| [dispose()](#dispose--) | Voert toepassingsgedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen. |
| [getInputBlockSize()](#getInputBlockSize--) | Haalt de invoerblokgrootte op. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Haalt de uitvoerblokgrootte op. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Transformeert het opgegeven gebied van de invoer-byte-array en kopieert de resulterende transformatie naar het opgegeven gebied van de uitvoer-byte-array. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Transformeert het opgegeven gebied van de opgegeven byte-array. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Haalt een waarde op die aangeeft of de huidige transformatie kan worden hergebruikt.

**Returns:**
boolean - een waarde die aangeeft of de huidige transformatie kan worden hergebruikt
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Haalt een waarde op die aangeeft of meerdere blokken kunnen worden getransformeerd.

**Returns:**
boolean - een waarde die aangeeft of meerdere blokken kunnen worden getransformeerd
### dispose() {#dispose--}
```
public abstract void dispose()
```


Voert toepassingsgedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Haalt de invoerblokgrootte op.

**Returns:**
int - de invoerblokgrootte
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Haalt de uitvoerblokgrootte op.

**Returns:**
int - de uitvoerblokgrootte
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Transformeert het opgegeven gebied van de invoer-byte-array en kopieert de resulterende transformatie naar het opgegeven gebied van de uitvoer-byte-array.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inputBuffer | byte[] | de invoer waarvoor de transformatie moet worden berekend |
| inputOffset | int | de offset in de invoer‑byte‑array vanaf waar gegevens worden gebruikt |
| inputCount | int | het aantal bytes in de invoer‑byte‑array dat als gegevens wordt gebruikt |
| outputBuffer | byte[] | de output waaraan de transformatie wordt geschreven |
| outputOffset | int | de offset in de output‑byte‑array vanaf waar gegevens worden geschreven |

**Returns:**
int - het aantal geschreven bytes
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Transformeert het opgegeven gebied van de opgegeven byte-array.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inputBuffer | byte[] | de invoer waarvoor de transformatie moet worden berekend |
| inputOffset | int | de offset in de invoer‑byte‑array vanaf waar gegevens worden gebruikt |
| inputCount | int | het aantal bytes in de invoer‑byte‑array dat als gegevens wordt gebruikt |

**Returns:**
byte[] - de berekende transformatie
