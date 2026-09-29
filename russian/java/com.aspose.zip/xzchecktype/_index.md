---
title: "XzCheckType"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Перечисление определяет подход к вычислению контрольной суммы для архива xz."
type: docs
weight: 170
url: /ru/java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

Перечисление определяет подход к вычислению контрольной суммы для архива xz.
## Поля

| Поле | Описание |
| --- | --- |
| [Crc32](#Crc32) | Контрольная сумма будет вычислена с использованием алгоритма CRC32. |
| [Crc64](#Crc64) | Контрольная сумма будет вычислена с использованием алгоритма CRC64. |
| [None](#None) | Контрольная сумма не будет вычислена. |
## Методы

| Метод | Описание |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


Контрольная сумма будет вычислена с использованием алгоритма CRC32.

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


Контрольная сумма будет вычислена с использованием алгоритма CRC64.

### None {#None}
```
public static final XzCheckType None
```


Контрольная сумма не будет вычислена.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
