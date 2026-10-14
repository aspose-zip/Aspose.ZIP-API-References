---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "항목을 압축하거나 압축 해제하는 데 사용되는 설정입니다."
type: docs
weight: 30
url: /ko/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

항목을 압축하거나 압축 해제하는 데 사용되는 설정입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | 새 인스턴스를 초기화합니다 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 클래스. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | 새 인스턴스를 초기화합니다 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 클래스. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | 새 인스턴스를 초기화합니다 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getComment()](#getComment--) | ZIP 아카이브 내 항목에 대한 주석을 가져옵니다. |
| [getCompressionSettings()](#getCompressionSettings--) | 압축 또는 압축 해제 루틴에 대한 설정을 가져옵니다. |
| [getEncryptionSettings()](#getEncryptionSettings--) | 암호화 또는 복호화에 대한 설정을 가져옵니다. |
| [setComment(String value)](#setComment-java.lang.String-) | ZIP 아카이브 내 항목에 대한 주석. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


새 인스턴스를 초기화합니다 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 클래스.

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


새 인스턴스를 초기화합니다 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 클래스.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | 압축 설정. 기본 deflate 설정을 위해 null을 전달합니다. |

다음 중 하나일 수 있습니다:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


새 인스턴스를 초기화합니다 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 클래스.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | 압축 설정. 기본 deflate 설정을 위해 null을 전달합니다. |

다음 중 하나일 수 있습니다:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | 암호화 설정. 암호화 또는 복호화가 필요 없을 경우 null을 전달합니다. |

다음 중 하나일 수 있습니다:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


ZIP 아카이브 내 항목에 대한 주석을 가져옵니다.

**Returns:**
java.lang.String - ZIP 아카이브 내 항목에 대한 주석.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


압축 또는 압축 해제 루틴에 대한 설정을 가져옵니다.

다음 중 하나일 수 있습니다:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


암호화 또는 복호화에 대한 설정을 가져옵니다. 특정 엔트리의 설정은 다를 수 있습니다.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


ZIP 아카이브 내 항목에 대한 주석.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

