---
title: "UueSaveOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры сохранения uuencoded файла."
type: docs
weight: 129
url: /ru/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Параметры сохранения uuencoded файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Инициализирует параметры именем файла, предоставленным пользователем, и новой строкой. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Инициализирует параметры именем файла, предоставленным пользователем, и строкой по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getFileName()](#getFileName--) | Получает имя файла, которое будет использоваться при воссоздании декодированных данных. |
| [getNewLine()](#getNewLine--) | Получает символ, завершающий каждую строку, обычно "\n" или "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Получает права доступа Unix файла. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Устанавливает Unix‑разрешения файла. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Инициализирует параметры именем файла, предоставленным пользователем, и новой строкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | имя файла, которое будет использоваться при воссоздании декодированных данных |
| newLine | java.lang.String | символ, завершающий каждую строку |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Инициализирует параметры именем файла, предоставленным пользователем, и строкой по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | имя файла, которое будет использоваться при воссоздании декодированных данных |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Получает имя файла, которое будет использоваться при воссоздании декодированных данных.

**Returns:**
java.lang.String — имя файла, которое будет использоваться при воссоздании декодированных данных
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Получает символ, завершающий каждую строку, обычно "\n" или "\r\n".

**Returns:**
java.lang.String — символ, завершающий каждую строку, обычно \"\\n\" или \"\\r\\n\".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Получает права доступа Unix файла.

По умолчанию 644.

**Returns:**
java.lang.String — Unix‑разрешения файла
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Устанавливает Unix‑разрешения файла.

По умолчанию 644.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Unix‑разрешения файла |

