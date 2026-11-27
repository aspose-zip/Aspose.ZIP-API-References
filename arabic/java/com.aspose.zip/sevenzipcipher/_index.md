---
title: "SevenZipCipher"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الفئة الأساسية لتشفير AES المستخدمة لتشفير 7-zip."
type: docs
weight: 110
url: /ar/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

الفئة الأساسية لتشفير AES المستخدمة لتشفير 7-zip.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | يحصل على قيمة تشير إلى ما إذا كان التحويل الحالي يمكن إعادة استخدامه. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | يحصل على قيمة تشير إلى ما إذا كان يمكن تحويل كتل متعددة. |
| [dispose()](#dispose--) | ينفذ مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [getInputBlockSize()](#getInputBlockSize--) | يحصل على حجم كتلة الإدخال. |
| [getOutputBlockSize()](#getOutputBlockSize--) | يحصل على حجم كتلة الإخراج. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | يحوّل المنطقة المحددة من مصفوفة البايتات الإدخالية وينسخ التحويل الناتج إلى المنطقة المحددة من مصفوفة البايتات الإخراجية. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | يحوّل المنطقة المحددة من مصفوفة البايتات المحددة. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


يحصل على قيمة تشير إلى ما إذا كان التحويل الحالي يمكن إعادة استخدامه.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان التحويل الحالي يمكن إعادة استخدامه
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


يحصل على قيمة تشير إلى ما إذا كان يمكن تحويل كتل متعددة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يمكن تحويل كتل متعددة
### dispose() {#dispose--}
```
public abstract void dispose()
```


ينفذ مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


يحصل على حجم كتلة الإدخال.

**Returns:**
int - حجم كتلة الإدخال
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


يحصل على حجم كتلة الإخراج.

**Returns:**
int - حجم كتلة الإخراج
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


يحوّل المنطقة المحددة من مصفوفة البايتات الإدخالية وينسخ التحويل الناتج إلى المنطقة المحددة من مصفوفة البايتات الإخراجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inputBuffer | byte[] | الإدخال الذي يُحسب له التحويل |
| inputOffset | int | الإزاحة في مصفوفة البايتات الإدخال التي يبدأ منها استخدام البيانات |
| inputCount | int | عدد البايتات في مصفوفة البايتات الإدخال التي تُستخدم كبيانات |
| outputBuffer | byte[] | الإخراج الذي يُكتب إليه التحويل |
| outputOffset | int | الإزاحة في مصفوفة البايتات الإخراج التي يبدأ منها كتابة البيانات |

**Returns:**
int - عدد البايتات المكتوبة
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


يحوّل المنطقة المحددة من مصفوفة البايتات المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inputBuffer | byte[] | الإدخال الذي يُحسب له التحويل |
| inputOffset | int | الإزاحة في مصفوفة البايتات الإدخال التي يبدأ منها استخدام البيانات |
| inputCount | int | عدد البايتات في مصفوفة البايتات الإدخال التي تُستخدم كبيانات |

**Returns:**
byte[] - التحويل المحسوب
