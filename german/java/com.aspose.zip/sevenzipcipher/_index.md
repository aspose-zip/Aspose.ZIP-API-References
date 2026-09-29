---
title: "SevenZipCipher"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Basisklasse für den AES-Chiffre, der für 7-zip-Verschlüsselung verwendet wird."
type: docs
weight: 110
url: /de/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Basisklasse für den AES-Chiffre, der für 7-zip-Verschlüsselung verwendet wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Gibt einen Wert zurück, der angibt, ob die aktuelle Transformation wiederverwendet werden kann. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Gibt einen Wert zurück, der angibt, ob mehrere Blöcke transformiert werden können. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [getInputBlockSize()](#getInputBlockSize--) | Gibt die Eingabeblockgröße zurück. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Gibt die Ausgabeblockgröße zurück. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Transformiert den angegebenen Bereich des Eingabe‑Byte‑Arrays und kopiert die resultierende Transformation in den angegebenen Bereich des Ausgabe‑Byte‑Arrays. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Transformiert den angegebenen Bereich des angegebenen Byte‑Arrays. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Gibt einen Wert zurück, der angibt, ob die aktuelle Transformation wiederverwendet werden kann.

**Returns:**
boolean - ein Wert, der angibt, ob die aktuelle Transformation wiederverwendet werden kann
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Gibt einen Wert zurück, der angibt, ob mehrere Blöcke transformiert werden können.

**Returns:**
boolean - ein Wert, der angibt, ob mehrere Blöcke transformiert werden können
### dispose() {#dispose--}
```
public abstract void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Gibt die Eingabeblockgröße zurück.

**Returns:**
int - die Eingabeblockgröße
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Gibt die Ausgabeblockgröße zurück.

**Returns:**
int - die Ausgabeblockgröße
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Transformiert den angegebenen Bereich des Eingabe‑Byte‑Arrays und kopiert die resultierende Transformation in den angegebenen Bereich des Ausgabe‑Byte‑Arrays.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inputBuffer | byte[] | die Eingabe, für die die Transformation berechnet werden soll |
| inputOffset | int | der Versatz im Eingabe‑Byte‑Array, ab dem Daten verwendet werden |
| inputCount | int | die Anzahl der Bytes im Eingabe‑Byte‑Array, die als Daten verwendet werden |
| outputBuffer | byte[] | die Ausgabe, in die die Transformation geschrieben wird |
| outputOffset | int | der Versatz im Ausgabe‑Byte‑Array, ab dem Daten geschrieben werden |

**Returns:**
int - die Anzahl der geschriebenen Bytes
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Transformiert den angegebenen Bereich des angegebenen Byte‑Arrays.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inputBuffer | byte[] | die Eingabe, für die die Transformation berechnet werden soll |
| inputOffset | int | der Versatz im Eingabe‑Byte‑Array, ab dem Daten verwendet werden |
| inputCount | int | die Anzahl der Bytes im Eingabe‑Byte‑Array, die als Daten verwendet werden |

**Returns:**
byte[] - die berechnete Transformation
