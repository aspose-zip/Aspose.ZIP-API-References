---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivi kaydetmek için seçenekler."
type: docs
weight: 36
url: /tr/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

ZIP arşivi kaydetmek için seçenekler.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip dosyası için isteğe bağlı yorumu alır. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Bir girdinin sıkıştırılmasının hemen ardından girdilerin kaynaklarının kapatılıp kapatılmayacağını gösteren değeri alır. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Veri Tanımlayıcı yayımı için ayarları alır. |
| [getEncoding()](#getEncoding--) | Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı alır. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Mevcut ZIP arşivini kaydetmek için şifreleme ayarlarını alır. |
| [getEventsBag()](#getEventsBag--) | Arşiv kaydedilirken tetiklenen olayların konteynerini alır. |
| [getParallelOptions()](#getParallelOptions--) | Paralel sıkıştırma için ayarları alır. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Kendiliğinden çıkarılan arşiv için ayarları alır. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip dosyası için isteğe bağlı yorumu ayarlar. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Bir giriş sıkıştırıldıktan hemen sonra girişlerin kaynaklarının kapatılıp kapanmayacağını belirten bir değer ayarlar. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Veri Tanımlayıcı yayını için ayarları belirler. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı ayarlar. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Mevcut ZIP arşivini kaydederken şifreleme ayarlarını belirler. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Arşiv kaydedilirken tetiklenen olayların konteynerini ayarlar. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Paralel sıkıştırma için ayarları belirler. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Kendiliğinden çıkarılan arşiv için ayarları belirler. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip dosyası için isteğe bağlı yorumu alır.

**Returns:**
java.lang.String - Zip dosyası için isteğe bağlı yorum.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Bir girdinin sıkıştırılmasının hemen ardından girdilerin kaynaklarının kapatılıp kapatılmayacağını gösteren değeri alır.

**Returns:**
boolean - Bir giriş sıkıştırıldıktan hemen sonra girişlerin kaynaklarının kapatılıp kapanmayacağını belirten bir değer.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Veri Tanımlayıcı yayımı için ayarları alır.

Varsayılan seçenek her zaman mevcut veri tanımlayıcıdır.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı alır.

Ayarlanmamışsa, kod sayfası 437 kullanılacaktır.

**Returns:**
java.nio.charset.Charset - Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlama.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Mevcut ZIP arşivini kaydetmek için şifreleme ayarlarını alır.

```

``````

try (Archive archive = new Archive(\"plain.zip\")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings(\"p@s$\", EncryptionMethod.AES256));
archive.save(\"encripted.zip\", options);
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

Şifreli arşivin normal oluşturulması için bu seçenekleri kullanmayın, kullanın

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) yerine.

`DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) değer olarak [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) olduğunda uyumlu değildir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Mevcut ZIP arşivini kaydederken şifreleme ayarlarını belirler. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Arşiv kaydedilirken tetiklenen olayların konteynerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | Arşiv kaydedilirken tetiklenen olayların konteyneri. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Paralel sıkıştırma için ayarları belirler.

Birden fazla arşiv girdisini sıkıştırırken birden fazla CPU çekirdeği kullanmak istiyorsanız atayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | Paralel sıkıştırma ayarları. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Kendiliğinden çıkarılan arşiv için ayarları belirler.

Hedef bilgisayara herhangi bir yazılım kurulmadan bir arşivi çıkarmak için çalıştırılabilir program oluşturmanız gerekiyorsa atayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | Kendiliğinden çıkarılan arşiv ayarları. |

