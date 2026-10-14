---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "7z 항목을 압축하거나 압축 해제하는 데 사용되는 설정."
type: docs
weight: 113
url: /ko/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

7z 항목을 압축하거나 압축 해제하는 데 사용되는 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | 새로운 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 클래스 인스턴스를 초기화합니다. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | 새로운 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 클래스 인스턴스를 초기화합니다. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | 새로운 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | 압축 파일 헤더를 압축할지 여부를 나타내는 값을 가져옵니다. |
| [getCompressionSettings()](#getCompressionSettings--) | 압축 또는 압축 해제 루틴에 대한 설정을 가져옵니다. |
| [getEncryptionSettings()](#getEncryptionSettings--) | 암호화 또는 복호화에 대한 설정을 가져옵니다. |
| [getSolid()](#getSolid--) | 엔트리를 연결하여 단일 데이터 블록으로 처리할지 여부를 나타내는 값을 가져옵니다. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | 압축 파일 헤더를 압축할지 여부를 나타내는 값을 설정합니다. |
| [setSolid(boolean value)](#setSolid-boolean-) | 엔트리를 연결하여 단일 데이터 블록으로 처리할지 여부를 나타내는 값을 설정합니다. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


새로운 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 클래스 인스턴스를 초기화합니다.

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


새로운 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | 압축 설정입니다. 기본 LZMA 설정을 사용하려면 null을 전달하십시오. |

다음 중 하나일 수 있습니다:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


새로운 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | 압축 설정입니다. 기본 LZMA 설정을 사용하려면 null을 전달하십시오. |

다음 중 하나일 수 있습니다:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | 암호화 설정입니다. 암호화 또는 복호화가 필요하지 않으면 null을 전달하십시오. |

하나만 지정할 수 있습니다:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


압축 파일 헤더를 압축할지 여부를 나타내는 값을 가져옵니다.

이 설정은 7-Zip 도구의 `-mhc=on` 스위치와 동일합니다. 현재 헤더 암호화와 호환되지 않습니다.

**Returns:**
boolean - 압축 파일 헤더를 압축할지 여부를 나타내는 값
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


압축 또는 압축 해제 루틴에 대한 설정을 가져옵니다.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


암호화 또는 복호화에 대한 설정을 가져옵니다. 특정 엔트리의 설정은 다를 수 있습니다.

[SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings)는 7z 아카이브에 대한 유일한 옵션입니다.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


엔트리를 연결하여 단일 데이터 블록으로 처리할지 여부를 나타내는 값을 가져옵니다.

다음 예제는 디렉터리를 암호화 없이 LZMA2 압축을 사용하여 솔리드 7z 아카이브로 압축하는 방법을 보여줍니다.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream(\"archive.7z\")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
try (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries(\"C:\\\\Documents\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

아카이브 인스턴스화 시 솔리드 7z 아카이브를 위해 `SevenZipEntrySettings`를 제공하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 엔트리를 연결하여 단일 데이터 블록으로 처리할지 여부를 나타내는 값. |

