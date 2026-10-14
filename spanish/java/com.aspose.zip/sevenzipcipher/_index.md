---
title: "SevenZipCipher"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Clase base para el cifrado AES utilizado para el cifrado 7-zip."
type: docs
weight: 110
url: /es/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Clase base para el cifrado AES utilizado para el cifrado 7-zip.
## Métodos

| Método | Descripción |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Obtiene un valor que indica si la transformación actual se puede reutilizar. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Obtiene un valor que indica si se pueden transformar varios bloques. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, la liberación o el restablecimiento de recursos no administrados. |
| [getInputBlockSize()](#getInputBlockSize--) | Obtiene el tamaño del bloque de entrada. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Obtiene el tamaño del bloque de salida. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Transforma la región especificada del arreglo de bytes de entrada y copia la transformación resultante a la región especificada del arreglo de bytes de salida. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Transforma la región especificada del arreglo de bytes especificado. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Obtiene un valor que indica si la transformación actual se puede reutilizar.

**Returns:**
boolean - un valor que indica si la transformación actual se puede reutilizar
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Obtiene un valor que indica si se pueden transformar varios bloques.

**Returns:**
boolean - un valor que indica si se pueden transformar varios bloques
### dispose() {#dispose--}
```
public abstract void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, la liberación o el restablecimiento de recursos no administrados.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Obtiene el tamaño del bloque de entrada.

**Returns:**
int - el tamaño del bloque de entrada
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Obtiene el tamaño del bloque de salida.

**Returns:**
int - el tamaño del bloque de salida
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Transforma la región especificada del arreglo de bytes de entrada y copia la transformación resultante a la región especificada del arreglo de bytes de salida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inputBuffer | byte[] | la entrada para la cual calcular la transformación |
| inputOffset | int | el desplazamiento en la matriz de bytes de entrada desde el cual comenzar a usar los datos |
| inputCount | int | el número de bytes en la matriz de bytes de entrada que se usarán como datos |
| outputBuffer | byte[] | la salida a la que escribir la transformación |
| outputOffset | int | el desplazamiento en la matriz de bytes de salida desde el cual comenzar a escribir datos |

**Returns:**
int - el número de bytes escritos
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Transforma la región especificada del arreglo de bytes especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inputBuffer | byte[] | la entrada para la cual calcular la transformación |
| inputOffset | int | el desplazamiento en la matriz de bytes de entrada desde el cual comenzar a usar los datos |
| inputCount | int | el número de bytes en la matriz de bytes de entrada que se usarán como datos |

**Returns:**
byte[] - la transformación calculada
