---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP अभिलेख को सहेजने के विकल्प।"
type: docs
weight: 36
url: /hi/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

ZIP अभिलेख को सहेजने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip फ़ाइल के लिए वैकल्पिक टिप्पणी प्राप्त करता है। |
| [getCloseEntrySource()](#getCloseEntrySource--) | एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं। |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Data Descriptor उत्सर्जन के लिए सेटिंग्स प्राप्त करता है। |
| [getEncoding()](#getEncoding--) | फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग प्राप्त करता है। |
| [getEncryptionOptions()](#getEncryptionOptions--) | मौजूदा ZIP संग्रह को सहेजने के लिए एन्क्रिप्शन सेटिंग्स प्राप्त करता है। |
| [getEventsBag()](#getEventsBag--) | आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को प्राप्त करता है। |
| [getParallelOptions()](#getParallelOptions--) | समांतर संपीड़न के लिए सेटिंग्स प्राप्त करता है। |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | स्वयं निकाले जाने वाले आर्काइव के लिए सेटिंग्स प्राप्त करता है। |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip फ़ाइल के लिए वैकल्पिक टिप्पणी सेट करता है। |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | एक मान सेट करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं। |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Data Descriptor उत्सर्जन के लिए सेटिंग्स सेट करता है। |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग सेट करता है। |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | मौजूदा ZIP संग्रह को सहेजने के लिए एन्क्रिप्शन सेटिंग्स सेट करता है। |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को सेट करता है। |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | समांतर संपीड़न के लिए सेटिंग्स सेट करता है। |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | स्वयं निकाले जाने वाले आर्काइव के लिए सेटिंग्स सेट करता है। |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip फ़ाइल के लिए वैकल्पिक टिप्पणी प्राप्त करता है।

**Returns:**
java.lang.String - ज़िप फ़ाइल के लिए वैकल्पिक टिप्पणी।
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि प्रविष्टियों के स्रोत को संपीड़ित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं।
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Data Descriptor उत्सर्जन के लिए सेटिंग्स प्राप्त करता है।

डिफ़ॉल्ट विकल्प हमेशा मौजूद डेटा डिस्क्रिप्टर होता है।

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग प्राप्त करता है।

यदि सेट नहीं किया गया, तो कोड पेज 437 उपयोग किया जाएगा।

**Returns:**
java.nio.charset.Charset - फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग।
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


मौजूदा ZIP संग्रह को सहेजने के लिए एन्क्रिप्शन सेटिंग्स प्राप्त करता है।

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

एन्क्रिप्टेड आर्काइव की सामान्य रचना के लिए इन विकल्पों का उपयोग न करें, उपयोग करें

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) के बजाय।

यह `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) के साथ संगत नहीं है, जिसका मान [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | मौजूदा ज़िप आर्काइव को सहेजने के लिए एन्क्रिप्शन सेटिंग्स सेट करता है। |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | आर्काइव सहेजने पर घटनाओं को उठाने वाला कंटेनर। |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


समांतर संपीड़न के लिए सेटिंग्स सेट करता है।

यदि आप कई आर्काइव प्रविष्टियों को संपीड़ित करते समय कई CPU कोर का उपयोग करना चाहते हैं तो इसे असाइन करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | समांतर संपीड़न के लिए सेटिंग्स। |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


स्वयं निकाले जाने वाले आर्काइव के लिए सेटिंग्स सेट करता है।

यदि आपको लक्ष्य कंप्यूटर पर कोई सॉफ़्टवेयर स्थापित किए बिना एक अभिलेख निकालने के लिए निष्पादन योग्य प्रोग्राम बनाना है तो इसे असाइन करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | स्वयं निकाले गए अभिलेख के लिए सेटिंग्स। |

