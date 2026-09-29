---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "내부에 항목을 구성하는 데 사용되는 설정."
type: docs
weight: 18
url: /ko/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

내부에 항목을 구성하는 데 사용되는 설정 [AppleArchive](../../com.aspose.zip/applearchive).
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | 새 인스턴스를 초기화합니다 [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | 구성된 Apple Archive 페이로드에 적용된 압축 설정을 가져옵니다. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | 구성된 파일 항목에 CRC32 체크섬 필드가 포함되는지 여부를 나타내는 값을 가져옵니다. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | 구성된 파일 항목에 CRC32 체크섬 필드가 포함되는지 여부를 나타내는 값을 설정합니다. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


새 인스턴스를 초기화합니다 [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) 클래스.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | 구성된 Apple Archive 페이로드에 적용된 압축 설정. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


구성된 Apple Archive 페이로드에 적용된 압축 설정을 가져옵니다.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


구성된 파일 항목에 CRC32 체크섬 필드가 포함되는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 구성된 파일 항목에 CRC32 체크섬 필드가 포함되는지 여부를 나타내는 값.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


구성된 파일 항목에 CRC32 체크섬 필드가 포함되는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 구성된 파일 항목에 CRC32 체크섬 필드가 포함되는지 여부를 나타내는 값. |

