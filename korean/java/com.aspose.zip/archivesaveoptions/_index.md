---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브를 저장하기 위한 옵션."
type: docs
weight: 36
url: /ko/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

ZIP 아카이브를 저장하기 위한 옵션.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip 파일에 대한 선택적 주석을 가져옵니다. |
| [getCloseEntrySource()](#getCloseEntrySource--) | 항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 가져옵니다. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Data Descriptor 방출에 대한 설정을 가져옵니다. |
| [getEncoding()](#getEncoding--) | 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 가져옵니다. |
| [getEncryptionOptions()](#getEncryptionOptions--) | 기존 ZIP 아카이브를 저장하기 위한 암호화 설정을 가져옵니다. |
| [getEventsBag()](#getEventsBag--) | 아카이브 저장 시 발생하는 이벤트 컨테이너를 가져옵니다. |
| [getParallelOptions()](#getParallelOptions--) | 병렬 압축에 대한 설정을 가져옵니다. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | 셀프 추출 아카이브에 대한 설정을 가져옵니다. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip 파일에 대한 선택적 주석을 설정합니다. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | 항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 설정합니다. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Data Descriptor 방출에 대한 설정을 설정합니다. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 설정합니다. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | 기존 ZIP 아카이브를 저장하기 위한 암호화 설정을 설정합니다. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | 아카이브 저장 시 발생하는 이벤트 컨테이너를 설정합니다. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | 병렬 압축에 대한 설정을 설정합니다. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | 셀프 추출 아카이브에 대한 설정을 설정합니다. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip 파일에 대한 선택적 주석을 가져옵니다.

**Returns:**
java.lang.String - Zip 파일에 대한 선택적 주석.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 항목이 압축된 직후에 항목의 소스를 닫아야 하는지를 나타내는 값.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Data Descriptor 방출에 대한 설정을 가져옵니다.

기본 옵션은 항상 존재하는 데이터 디스크립터입니다.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 가져옵니다.

설정되지 않으면 코드 페이지 437이 사용됩니다.

**Returns:**
java.nio.charset.Charset - 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


기존 ZIP 아카이브를 저장하기 위한 암호화 설정을 가져옵니다.

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

암호화된 아카이브를 일반적으로 구성할 때 이 옵션을 사용하지 말고, 사용하십시오

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) 대신.

`DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) 값이 [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)인 경우 호환되지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | 기존 ZIP 아카이브를 저장하기 위한 암호화 설정을 지정합니다. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


아카이브 저장 시 발생하는 이벤트 컨테이너를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | 아카이브 저장 시 발생하는 이벤트를 담는 컨테이너. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


병렬 압축에 대한 설정을 설정합니다.

여러 아카이브 항목을 압축하는 동안 여러 CPU 코어를 활용하려면 이를 할당하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | 병렬 압축을 위한 설정. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


셀프 추출 아카이브에 대한 설정을 설정합니다.

대상 컴퓨터에 소프트웨어가 설치되지 않은 상태에서 아카이브를 추출하기 위한 실행 프로그램을 작성해야 할 경우 이를 할당하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | 셀프 추출 아카이브에 대한 설정. |

