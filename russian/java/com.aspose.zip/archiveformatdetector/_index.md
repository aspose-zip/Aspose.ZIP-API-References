---
title: "ArchiveFormatDetector"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Определяет формат архива и предоставляет другую связанную информацию."
type: docs
weight: 32
url: /ru/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Определяет формат архива и предоставляет другую связанную информацию.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Инициализирует новый экземпляр класса [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Методы

| Метод | Описание |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Получает информацию о формате. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Получает информацию о формате. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Инициализирует новый экземпляр класса [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Получает информацию о формате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток архивного файла. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Получает информацию о формате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
