---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att spara ett ZIP-arkiv."
type: docs
weight: 36
url: /sv/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Alternativ för att spara ett ZIP-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Hämtar valfri kommentar för Zip-filen. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Hämtar ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Hämtar inställningar för utsändning av Data Descriptor. |
| [getEncoding()](#getEncoding--) | Hämtar kodning för att konvertera filnamn och andra strängar till byte. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Hämtar krypteringsinställningar för att spara befintligt ZIP-arkiv. |
| [getEventsBag()](#getEventsBag--) | Hämtar behållare för händelser som utlöses vid arkivsparning. |
| [getParallelOptions()](#getParallelOptions--) | Hämtar inställningar för parallell komprimering. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Hämtar inställningar för självextraherande arkiv. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Ställer in valfri kommentar för Zip-filen. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Ställer in ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Ställer in inställningar för utsändning av Data Descriptor. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ställer in kodning för att konvertera filnamn och andra strängar till byte. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Ställer in krypteringsinställningar för att spara befintligt ZIP-arkiv. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Ställer in behållare för händelser som utlöses vid arkivsparning. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Ställer in inställningar för parallell komprimering. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Ställer in inställningar för självextraherande arkiv. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Hämtar valfri kommentar för Zip-filen.

**Returns:**
java.lang.String - valfri kommentar för Zip-filen.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Hämtar ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats.

**Returns:**
boolean - ett värde som indikerar om källorna för poster ska stängas direkt efter att en post har komprimerats.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Hämtar inställningar för utsändning av Data Descriptor.

Standardalternativet är alltid en närvarande databeskrivare.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Hämtar kodning för att konvertera filnamn och andra strängar till byte.

Om den inte är angiven används kodsidan 437.

**Returns:**
java.nio.charset.Charset - kodning för att konvertera filnamn och andra strängar till byte.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Hämtar krypteringsinställningar för att spara befintligt ZIP-arkiv.

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

Använd inte dessa alternativ för vanlig sammansättning av krypterat arkiv, använd

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) istället.

Inte kompatibel med `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) med värdet [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | av sätter krypteringsinställningar för att spara ett befintligt ZIP-arkiv. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Ställer in behållare för händelser som utlöses vid arkivsparning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | behållare för händelser som utlöses vid arkivlagring. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Ställer in inställningar för parallell komprimering.

Tilldela den om du vill utnyttja flera CPU-kärnor medan du komprimerar flera arkivposter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | inställningar för parallell komprimering. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Ställer in inställningar för självextraherande arkiv.

Tilldela det om du behöver skapa ett körbart program för att extrahera ett arkiv utan någon programvara installerad på mål‑datorn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | inställningar för självextraherat arkiv. |

