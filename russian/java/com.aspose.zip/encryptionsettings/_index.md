---
title: "EncryptionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Базовый класс для настроек нескольких методов шифрования ZIP."
type: docs
weight: 60
url: /ru/java/com.aspose.zip/encryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class EncryptionSettings
```

Базовый класс для настроек нескольких методов шифрования ZIP.
## Методы

| Метод | Описание |
| --- | --- |
| [getMethod()](#getMethod--) | Получает алгоритм шифрования. |
| [getPassword()](#getPassword--) | Возвращает пароль для шифрования или расшифровки. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для шифрования или расшифровки. |
### getMethod() {#getMethod--}
```
public final EncryptionMethod getMethod()
```


Получает алгоритм шифрования.

**Returns:**
[EncryptionMethod](../../com.aspose.zip/encryptionmethod) - the encryption algorithm.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Возвращает пароль для шифрования или расшифровки.

**Returns:**
java.lang.String - пароль для шифрования или дешифрования.
### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Устанавливает пароль для шифрования или расшифровки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | пароль для шифрования или дешифрования. |

