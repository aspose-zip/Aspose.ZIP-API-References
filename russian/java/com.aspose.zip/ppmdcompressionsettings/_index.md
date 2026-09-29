---
title: "PPMdCompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия PPMd внутри ZIP-архива."
type: docs
weight: 93
url: /ru/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Настройки сжатия PPMd внутри ZIP-архива.

PPMd — это алгоритм сжатия данных, разработанный Дмитрием Шкарином. Этот алгоритм основан на предиктивном сопоставлении фраз в контекстах нескольких порядков.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Инициализирует новый экземпляр класса [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Инициализирует новый экземпляр класса [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) с порядком модели и размером субаллокатора по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Получает порядок модели. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Получает размер субаллокации в МБ. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Инициализирует новый экземпляр класса [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

Порядок модели по умолчанию — 8, а размер субаллокатора — 50 МБ.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Получает порядок модели.

**Returns:**
int — порядок модели
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Получает размер субаллокации в МБ.

**Returns:**
int - размер субаллокации в МБ
