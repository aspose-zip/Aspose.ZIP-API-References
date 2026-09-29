---
title: "ArchiveSaveOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk menyimpan arsip ZIP."
type: docs
weight: 36
url: /id/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Opsi untuk menyimpan arsip ZIP.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Mendapatkan komentar opsional untuk file Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Mendapatkan nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Mendapatkan pengaturan untuk emisi Data Descriptor. |
| [getEncoding()](#getEncoding--) | Mendapatkan enkoding untuk mengonversi nama file dan string lainnya menjadi byte. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Mendapatkan pengaturan enkripsi untuk menyimpan arsip ZIP yang ada. |
| [getEventsBag()](#getEventsBag--) | Mendapatkan kontainer peristiwa yang dipicu saat menyimpan arsip. |
| [getParallelOptions()](#getParallelOptions--) | Mendapatkan pengaturan untuk kompresi paralel. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Mendapatkan pengaturan untuk arsip yang dapat mengekstrak sendiri. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Mengatur komentar opsional untuk file Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Mengatur nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Mengatur pengaturan untuk emisi Data Descriptor. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur enkoding untuk mengonversi nama file dan string lainnya menjadi byte. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Mengatur pengaturan enkripsi untuk menyimpan arsip ZIP yang ada. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Mengatur kontainer peristiwa yang dipicu saat menyimpan arsip. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Mengatur pengaturan untuk kompresi paralel. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Mengatur pengaturan untuk arsip yang dapat mengekstrak sendiri. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Mendapatkan komentar opsional untuk file Zip.

**Returns:**
java.lang.String - komentar opsional untuk file Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Mendapatkan nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi.

**Returns:**
boolean - nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah sebuah entri dikompresi.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Mendapatkan pengaturan untuk emisi Data Descriptor.

Opsi default selalu menyertakan deskriptor data.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Mendapatkan enkoding untuk mengonversi nama file dan string lainnya menjadi byte.

Jika tidak disetel, kode halaman 437 akan digunakan.

**Returns:**
java.nio.charset.Charset - pengkodean untuk mengonversi nama file dan string lainnya menjadi byte.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Mendapatkan pengaturan enkripsi untuk menyimpan arsip ZIP yang ada.

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

Jangan gunakan opsi ini untuk komposisi biasa arsip terenkripsi, gunakan

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) sebagai gantinya.

Tidak kompatibel dengan `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) yang memiliki nilai [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | menetapkan pengaturan enkripsi untuk menyimpan arsip ZIP yang ada. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Mengatur kontainer peristiwa yang dipicu saat menyimpan arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | kontainer peristiwa yang dipicu saat menyimpan arsip. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Mengatur pengaturan untuk kompresi paralel.

Tetapkan jika Anda ingin memanfaatkan beberapa inti CPU saat mengompresi beberapa entri arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | pengaturan untuk kompresi paralel. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Mengatur pengaturan untuk arsip yang dapat mengekstrak sendiri.

Tetapkan jika Anda perlu membuat program yang dapat dijalankan untuk mengekstrak arsip tanpa perangkat lunak apa pun yang terpasang di komputer target.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | pengaturan untuk arsip yang diekstrak sendiri. |

