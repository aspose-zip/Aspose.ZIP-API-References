---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры сохранения многотомного архива 7-zip."
type: docs
weight: 123
url: /ru/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Параметры сохранения многотомного архива 7-zip.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Создает настройки для сохранения многотомного архива 7z. |
## Методы

| Метод | Описание |
| --- | --- |
| [getFileName()](#getFileName--) | Получает имя сегментов без расширения. |
| [getSegmentSize()](#getSegmentSize--) | Получает размер сегмента. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Создает настройки для сохранения многотомного архива 7z.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileName | java.lang.String | Имя томов. Может быть с расширением .7z или без него. |

Имена файлов будут следующими: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | Размер тома. |

Некоторые тома могут быть меньше, чем `segmentSize`. В большинстве случаев последний сегмент будет меньше, но иногда обычные сегменты тоже могут быть меньше. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Получает имя сегментов без расширения.

**Returns:**
java.lang.String — имя сегментов без расширения
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Получает размер сегмента.

**Returns:**
long — размер сегмента.
