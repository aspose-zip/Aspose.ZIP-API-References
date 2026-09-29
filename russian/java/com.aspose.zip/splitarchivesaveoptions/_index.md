---
title: "SplitArchiveSaveOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры сохранения многотомного архива ZIP."
type: docs
weight: 122
url: /ru/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Параметры сохранения многотомного архива ZIP.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Создает экземпляр настроек для сохранения многотомного ZIP-архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Получает необязательный комментарий для Zip‑файла. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Получает значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи. |
| [getEncoding()](#getEncoding--) | Получает кодировку для преобразования имён файлов и других строк в байты. |
| [getEventsBag()](#getEventsBag--) | Получает контейнер событий, возникающих при сохранении архива. |
| [getFileName()](#getFileName--) | Получает имя сегментов без расширения. |
| [getSegmentSize()](#getSegmentSize--) | Получает размер сегмента. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Устанавливает необязательный комментарий для Zip‑файла. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Устанавливает значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Устанавливает кодировку для преобразования имён файлов и других строк в байты. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Устанавливает контейнер событий, возникающих при сохранении архива. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Создает экземпляр настроек для сохранения многотомного ZIP-архива.

Некоторые тома могут быть меньше, чем `segmentSize`. В большинстве случаев последний сегмент будет меньше, но редко обычные сегменты могут быть тоже меньше.

Имена файлов будут следующими: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя томов. Может быть с расширением .zip или без него. |
| segmentSize | long | Размер тома. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Получает необязательный комментарий для Zip‑файла.

**Returns:**
java.lang.String - необязательный комментарий для Zip‑файла.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Получает значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи.

**Returns:**
boolean - значение, указывающее, следует ли закрывать источники записей сразу после того, как запись была сжата.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Получает кодировку для преобразования имён файлов и других строк в байты.

Если не задано, будет использоваться кодовая страница 437.

**Returns:**
java.nio.charset.Charset - кодировка для преобразования имён файлов и других строк в байты.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Получает контейнер событий, возникающих при сохранении архива.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Получает имя сегментов без расширения.

**Returns:**
java.lang.String — имя сегментов без расширения.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Получает размер сегмента.

**Returns:**
long — размер сегмента.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Устанавливает необязательный комментарий для Zip‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | необязательный комментарий для Zip‑файла. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Устанавливает значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Устанавливает кодировку для преобразования имён файлов и других строк в байты.

Если не задано, будет использоваться кодовая страница 437.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.nio.charset.Charset | кодировка для преобразования имен файлов и других строк в байты. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Устанавливает контейнер событий, возникающих при сохранении архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | контейнер событий, возникающих при сохранении архива. |

