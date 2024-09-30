---
title: ArchiveSaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving a zip archive.
type: docs
weight: 20
url: /java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Options for saving a zip archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Gets optional comment for the Zip file. |
| [getEncoding()](#getEncoding--) | Gets encoding for converting file names and other strings to bytes. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Gets encryption settings for saving existing zip archive. |
| [getEventsBag()](#getEventsBag--) | Gets container of events raising on archive saving. |
| [getParallelOptions()](#getParallelOptions--) | Gets settings for parallel compression. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Gets settings for self extracted archive. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Sets optional comment for the Zip file. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets encoding for converting file names and other strings to bytes. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Sets encryption settings for saving existing zip archive. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Sets container of events raising on archive saving. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Sets settings for parallel compression. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Sets settings for self extracted archive. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Gets optional comment for the Zip file.

**Returns:**
java.lang.String - optional comment for the Zip file.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Returns:**
java.nio.charset.Charset - encoding for converting file names and other strings to bytes.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Gets encryption settings for saving existing zip archive.

```

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

Do not use this options for regular composition of encrypted archive.

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing zip archive.
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


Sets encryption settings for saving existing zip archive.

```

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

Do not use this options for regular composition of encrypted archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | encryption settings for saving existing zip archive. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Sets container of events raising on archive saving.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | container of events raising on archive saving. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Sets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | settings for parallel compression. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Sets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | settings for self extracted archive. |

