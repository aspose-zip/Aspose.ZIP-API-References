---
title: "SevenZipPPMdCompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки метода сжатия PPMd внутри 7z‑архива."
type: docs
weight: 117
url: /ru/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Настройки метода сжатия PPMd внутри 7z‑архива.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Создаёт настройки метода сжатия PPMd в архиве 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Создаёт настройки метода сжатия PPMd в архиве 7z с порядком модели по умолчанию и размером субаллокации. |
## Методы

| Метод | Описание |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Получает максимальный порядок. |
| [getMethod()](#getMethod--) | Получает метод сжатия или распаковки. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Получает размер субаллокации в МБ. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Создаёт настройки метода сжатия PPMd в архиве 7z.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

Порядок модели по умолчанию равен 6, а размер субаллокации — 16 МБ.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Получает максимальный порядок.

**Returns:**
byte - максимальный порядок
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Получает метод сжатия или распаковки.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Получает размер субаллокации в МБ.

**Returns:**
int - размер субаллокации в МБ
