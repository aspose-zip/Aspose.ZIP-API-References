---
title: "SevenZipCipher"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Базовый класс для шифра AES, используемого в шифровании 7‑zip."
type: docs
weight: 110
url: /ru/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Базовый класс для шифра AES, используемого в шифровании 7‑zip.
## Методы

| Метод | Описание |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Возвращает значение, указывающее, может ли текущая трансформация быть переиспользована. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Возвращает значение, указывающее, могут ли быть преобразованы несколько блоков. |
| [dispose()](#dispose--) | Выполняет определённые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [getInputBlockSize()](#getInputBlockSize--) | Возвращает размер входного блока. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Возвращает размер выходного блока. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Преобразует указанную область входного массива байтов и копирует полученную трансформацию в указанную область выходного массива байтов. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Преобразует указанную область указанного массива байтов. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Возвращает значение, указывающее, может ли текущая трансформация быть переиспользована.

**Returns:**
boolean - значение, указывающее, может ли текущая трансформация быть переиспользована
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Возвращает значение, указывающее, могут ли быть преобразованы несколько блоков.

**Returns:**
boolean - значение, указывающее, могут ли быть преобразованы несколько блоков
### dispose() {#dispose--}
```
public abstract void dispose()
```


Выполняет определённые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Возвращает размер входного блока.

**Returns:**
int - размер входного блока
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Возвращает размер выходного блока.

**Returns:**
int - размер выходного блока
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Преобразует указанную область входного массива байтов и копирует полученную трансформацию в указанную область выходного массива байтов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inputBuffer | byte[] | входные данные, для которых необходимо вычислить трансформацию |
| inputOffset | int | смещение в массиве входных байтов, с которого начинать использовать данные |
| inputCount | int | число байтов во входном массиве байтов, используемых в качестве данных |
| outputBuffer | byte[] | выход, в который записывается преобразование |
| outputOffset | int | смещение в массиве выходных байтов, с которого начинать запись данных |

**Returns:**
int - количество записанных байтов
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Преобразует указанную область указанного массива байтов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inputBuffer | byte[] | входные данные, для которых необходимо вычислить трансформацию |
| inputOffset | int | смещение в массиве входных байтов, с которого начинать использовать данные |
| inputCount | int | число байтов во входном массиве байтов, используемых в качестве данных |

**Returns:**
byte[] - вычисленное преобразование
