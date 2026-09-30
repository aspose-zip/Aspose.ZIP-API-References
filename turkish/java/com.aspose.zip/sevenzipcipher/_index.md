---
title: "SevenZipCipher"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7-zip şifrelemesi için kullanılan AES şifreleyicisinin temel sınıfı."
type: docs
weight: 110
url: /tr/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

7-zip şifrelemesi için kullanılan AES şifreleyicisinin temel sınıfı.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Geçerli dönüşümün yeniden kullanılabilir olup olmadığını gösteren bir değeri alır. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Birden fazla bloğun dönüştürülebilir olup olmadığını gösteren bir değeri alır. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [getInputBlockSize()](#getInputBlockSize--) | Giriş blok boyutunu alır. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Çıkış blok boyutunu alır. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Giriş bayt dizisinin belirtilen bölgesini dönüştürür ve ortaya çıkan dönüşümü çıkış bayt dizisinin belirtilen bölgesine kopyalar. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Belirtilen bayt dizisinin belirtilen bölgesini dönüştürür. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Geçerli dönüşümün yeniden kullanılabilir olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean - geçerli dönüşümün yeniden kullanılabilir olup olmadığını gösteren bir değer
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Birden fazla bloğun dönüştürülebilir olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean - birden fazla bloğun dönüştürülebileceğini gösteren bir değer
### dispose() {#dispose--}
```
public abstract void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Giriş blok boyutunu alır.

**Returns:**
int - giriş bloğu boyutu
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Çıkış blok boyutunu alır.

**Returns:**
int - çıkış bloğu boyutu
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Giriş bayt dizisinin belirtilen bölgesini dönüştürür ve ortaya çıkan dönüşümü çıkış bayt dizisinin belirtilen bölgesine kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inputBuffer | byte[] | dönüşümün hesaplanacağı girdi |
| inputOffset | int | veri kullanılmaya başlanacak giriş bayt dizisinin ofseti |
| inputCount | int | veri olarak kullanılacak giriş bayt dizisindeki bayt sayısı |
| outputBuffer | byte[] | dönüşümün yazılacağı çıktı |
| outputOffset | int | veri yazılmaya başlanacak çıkış bayt dizisinin ofseti |

**Returns:**
int - yazılan bayt sayısı
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Belirtilen bayt dizisinin belirtilen bölgesini dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inputBuffer | byte[] | dönüşümün hesaplanacağı girdi |
| inputOffset | int | veri kullanılmaya başlanacak giriş bayt dizisinin ofseti |
| inputCount | int | veri olarak kullanılacak giriş bayt dizisindeki bayt sayısı |

**Returns:**
byte[] - hesaplanmış dönüşüm
