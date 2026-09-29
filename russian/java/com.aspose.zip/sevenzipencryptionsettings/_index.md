---
title: "SevenZipEncryptionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Базовый класс для настроек нескольких методов шифрования 7z."
type: docs
weight: 112
url: /ru/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Базовый класс для настроек нескольких методов шифрования 7z.

AES-256 является единственным возможным методом шифрования для 7z архива. Поэтому [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) является единственной реализацией.
## Методы

| Метод | Описание |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Возвращает значение, указывающее на шифрование заголовка. |
| [getPassword()](#getPassword--) | Возвращает пароль для шифрования или расшифровки. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Устанавливает значение, указывающее на шифрование заголовка. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для шифрования или расшифровки. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Возвращает значение, указывающее на шифрование заголовка.

Эта настройка эквивалентна переключателю `-mhe=on` инструмента 7-Zip. В настоящее время она несовместима со сжатием заголовка.

**Returns:**
boolean - значение, указывающее на шифрование заголовка
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Возвращает пароль для шифрования или расшифровки.

**Returns:**
java.lang.String - пароль для шифрования или расшифровки
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Устанавливает значение, указывающее на шифрование заголовка.

Эта настройка эквивалентна переключателю `-mhe=on` инструмента 7-Zip. В настоящее время она несовместима со сжатием заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее на шифрование заголовка |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Устанавливает пароль для шифрования или расшифровки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | пароль для шифрования или расшифровки |

