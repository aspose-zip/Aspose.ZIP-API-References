---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het opslaan van een ZIP-archief."
type: docs
weight: 36
url: /nl/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Opties voor het opslaan van een ZIP-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Haalt optionele opmerking op voor het Zip‑bestand. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Haalt een waarde op die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Haalt instellingen op voor het uitgeven van Data Descriptor. |
| [getEncoding()](#getEncoding--) | Haalt codering op voor het converteren van bestandsnamen en andere tekenreeksen naar bytes. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Haalt encryptie‑instellingen op voor het opslaan van een bestaande ZIP‑archief. |
| [getEventsBag()](#getEventsBag--) | Haalt container van gebeurtenissen op die worden geactiveerd bij het opslaan van een archief. |
| [getParallelOptions()](#getParallelOptions--) | Haalt instellingen op voor parallelle compressie. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Haalt instellingen op voor zelfuitpakkend archief. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Stelt optionele opmerking in voor het Zip‑bestand. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Stelt een waarde in die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Stelt instellingen in voor het uitgeven van Data Descriptor. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Stelt codering in voor het converteren van bestandsnamen en andere tekenreeksen naar bytes. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Stelt encryptie‑instellingen in voor het opslaan van een bestaande ZIP‑archief. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Stelt container van gebeurtenissen in die worden geactiveerd bij het opslaan van een archief. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Stelt instellingen in voor parallelle compressie. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Stelt instellingen in voor zelfuitpakkend archief. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Haalt optionele opmerking op voor het Zip‑bestand.

**Returns:**
java.lang.String - optionele opmerking voor het Zip-bestand.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Haalt een waarde op die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten.

**Returns:**
boolean - een waarde die aangeeft of de bronnen van items moeten worden gesloten direct nadat een item is gecomprimeerd.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Haalt instellingen op voor het uitgeven van Data Descriptor.

Standaardoptie is altijd aanwezige data-descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Haalt codering op voor het converteren van bestandsnamen en andere tekenreeksen naar bytes.

Indien niet ingesteld, wordt codepagina 437 gebruikt.

**Returns:**
java.nio.charset.Charset - codering voor het converteren van bestandsnamen en andere strings naar bytes.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Haalt encryptie‑instellingen op voor het opslaan van een bestaande ZIP‑archief.

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

Gebruik deze opties niet voor de reguliere samenstelling van een versleuteld archief, gebruik

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) in plaats daarvan.

Niet compatibel met `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) met waarde [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | of stelt encryptie‑instellingen in voor het opslaan van een bestaand ZIP‑archief. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Stelt container van gebeurtenissen in die worden geactiveerd bij het opslaan van een archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | container van gebeurtenissen die worden getriggerd bij het opslaan van een archief. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Stelt instellingen in voor parallelle compressie.

Wijs het toe als je meerdere CPU‑kernen wilt gebruiken tijdens het comprimeren van meerdere archief‑items.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | instellingen voor parallelle compressie. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Stelt instellingen in voor zelfuitpakkend archief.

Wijs het toe als je een uitvoerbaar programma moet samenstellen om een archief te extraheren zonder enige software geïnstalleerd op de doelcomputer.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | instellingen voor zelfuitpakkend archief. |

