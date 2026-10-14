---
title: "Bzip2CompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия Bzip2 внутри ZIP‑архива."
type: docs
weight: 41
url: /ru/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Настройки сжатия Bzip2 внутри ZIP‑архива.

bzip2 сжимает файлы, используя алгоритм сортировки блоков текста Burrows-Wheeler и кодирование Хаффмана.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Создаёт новый экземпляр класса [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Создаёт новый экземпляр класса [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) с размером блока по умолчанию, равным 9 сотням килобайт. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Размер блока в сотнях килобайт. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Создаёт новый экземпляр класса [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Размер блока в сотнях килобайт.

**Returns:**
int — размер блока в сотнях килобайт
