---
title: "SevenZipCipher"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Classe de base pour le chiffrement AES utilisé pour le chiffrement 7-zip."
type: docs
weight: 110
url: /fr/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Classe de base pour le chiffrement AES utilisé pour le chiffrement 7-zip.
## Méthodes

| Méthode | Description |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Obtient une valeur indiquant si la transformation actuelle peut être réutilisée. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Obtient une valeur indiquant si plusieurs blocs peuvent être transformés. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [getInputBlockSize()](#getInputBlockSize--) | Obtient la taille du bloc d'entrée. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Obtient la taille du bloc de sortie. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Transforme la région spécifiée du tableau d'octets d'entrée et copie la transformation résultante dans la région spécifiée du tableau d'octets de sortie. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Transforme la région spécifiée du tableau d'octets spécifié. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Obtient une valeur indiquant si la transformation actuelle peut être réutilisée.

**Returns:**
boolean - une valeur indiquant si la transformation actuelle peut être réutilisée
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Obtient une valeur indiquant si plusieurs blocs peuvent être transformés.

**Returns:**
boolean - une valeur indiquant si plusieurs blocs peuvent être transformés
### dispose() {#dispose--}
```
public abstract void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Obtient la taille du bloc d'entrée.

**Returns:**
int - la taille du bloc d'entrée
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Obtient la taille du bloc de sortie.

**Returns:**
int - la taille du bloc de sortie
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Transforme la région spécifiée du tableau d'octets d'entrée et copie la transformation résultante dans la région spécifiée du tableau d'octets de sortie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inputBuffer | byte[] | l'entrée pour laquelle calculer la transformation |
| inputOffset | int | le décalage dans le tableau d'octets d'entrée à partir duquel commencer à utiliser les données |
| inputCount | int | le nombre d'octets dans le tableau d'octets d'entrée à utiliser comme données |
| outputBuffer | byte[] | la sortie dans laquelle écrire la transformation |
| outputOffset | int | le décalage dans le tableau d'octets de sortie à partir duquel commencer à écrire les données |

**Returns:**
int - le nombre d'octets écrits
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Transforme la région spécifiée du tableau d'octets spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inputBuffer | byte[] | l'entrée pour laquelle calculer la transformation |
| inputOffset | int | le décalage dans le tableau d'octets d'entrée à partir duquel commencer à utiliser les données |
| inputCount | int | le nombre d'octets dans le tableau d'octets d'entrée à utiliser comme données |

**Returns:**
byte[] - la transformation calculée
