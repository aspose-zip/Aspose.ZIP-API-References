---
title: "GzipLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры загрузки ."
type: docs
weight: 70
url: /ru/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Параметры загрузки [GzipArchive](../../com.aspose.zip/gziparchive).

В .NET Framework 4.0 и выше может использоваться для отмены извлечения.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Получает значение, указывающее, следует ли разбирать заголовок потока для определения свойств, включая имя. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Устанавливает значение, указывающее, следует ли разбирать заголовок потока для определения свойств, включая имя. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Получает значение, указывающее, следует ли разбирать заголовок потока для определения свойств, включая имя. Имеет смысл только для потоков, поддерживающих поиск.

**Returns:**
boolean - значение, указывающее, следует ли разбирать заголовок потока для определения свойств, включая имя.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Устанавливает флаг отмены, используемый для отмены операции извлечения.

Отменить извлечение gzip-архива после определённого времени.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println(\"Extraction was cancelled after 60 seconds\");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

