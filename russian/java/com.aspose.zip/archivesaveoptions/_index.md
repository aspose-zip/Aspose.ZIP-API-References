---
title: "ArchiveSaveOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры сохранения ZIP‑архива."
type: docs
weight: 36
url: /ru/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Параметры сохранения ZIP‑архива.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Получает необязательный комментарий для Zip‑файла. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Получает значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Получает настройки для генерации дескриптора данных. |
| [getEncoding()](#getEncoding--) | Получает кодировку для преобразования имён файлов и других строк в байты. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Получает настройки шифрования для сохранения существующего ZIP‑архива. |
| [getEventsBag()](#getEventsBag--) | Получает контейнер событий, возникающих при сохранении архива. |
| [getParallelOptions()](#getParallelOptions--) | Получает настройки параллельного сжатия. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Получает настройки самораспаковывающегося архива. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Устанавливает необязательный комментарий для Zip‑файла. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Устанавливает значение, указывающее, следует ли закрывать источники записей сразу после сжатия записи. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Устанавливает настройки для генерации дескриптора данных. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Устанавливает кодировку для преобразования имён файлов и других строк в байты. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Устанавливает настройки шифрования для сохранения существующего ZIP‑архива. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Устанавливает контейнер событий, возникающих при сохранении архива. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Устанавливает настройки параллельного сжатия. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Устанавливает настройки самораспаковывающегося архива. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


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
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Получает настройки для генерации дескриптора данных.

Опция по умолчанию всегда содержит дескриптор данных.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Получает кодировку для преобразования имён файлов и других строк в байты.

Если не задано, будет использоваться кодовая страница 437.

**Returns:**
java.nio.charset.Charset - кодировка для преобразования имён файлов и других строк в байты.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Получает настройки шифрования для сохранения существующего ZIP‑архива.

```

``````

try (Archive archive = new Archive("plain.zip")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
archive.save("encripted.zip", options);
}
 
```

Do not use this options for regular composition of encrypted archive, use

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) instead.

Not compatible with `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) having value [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing ZIP archive.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### getSelfExtractorOptions() {#getSelfExtractorOptions--}
```
public final SelfExtractorOptions getSelfExtractorOptions()
```


Gets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Returns:**
[SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) - settings for self extracted archive.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Sets a value indicating whether entries' sources should be closed right after an entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether entries' sources should be closed right after an entry has been compressed. |

### setDataDescriptorPolicy(ZipDataDescriptorPolicy value) {#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-}
```
public final void setDataDescriptorPolicy(ZipDataDescriptorPolicy value)
```


Sets settings for Data Descriptor emission.

Default option is always present data descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) | settings for Data Descriptor emission. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEncryptionOptions(EncryptionSettings value) {#setEncryptionOptions-com.aspose.zip.EncryptionSettings-}
```
public final void setEncryptionOptions(EncryptionSettings value)
```


Sets encryption settings for saving existing ZIP archive.

```

``````

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

Не используйте эти параметры для обычного создания зашифрованного архива, используйте

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) вместо этого.

Не совместимо с `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) при значении [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | устанавливает параметры шифрования для сохранения существующего ZIP‑архива. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Устанавливает контейнер событий, возникающих при сохранении архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | контейнер событий, возникающих при сохранении архива. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Устанавливает настройки параллельного сжатия.

Назначьте его, если хотите использовать несколько ядер CPU при сжатии нескольких записей архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | параметры параллельного сжатия. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Устанавливает настройки самораспаковывающегося архива.

Назначьте его, если вам нужно создать исполняемую программу для извлечения архива без установки какого-либо программного обеспечения на целевом компьютере.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | настройки для самораспаковывающегося архива. |

