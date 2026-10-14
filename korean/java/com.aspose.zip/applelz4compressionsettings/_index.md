---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "Apple Archive .aar 파일 내 LZ4 압축 설정."
type: docs
weight: 21
url: /ko/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) 파일 내 LZ4 압축에 대한 설정입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | 새로운 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 클래스 인스턴스를 초기화합니다. |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | 기본 매개변수로 새로운 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | `pbz4`/`bv41` 압축 블록 각각의 크기를 가져옵니다. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


새로운 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | int | 각 압축된 `pbz4`/`bv41` 블록의 크기. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


기본 매개변수로 새로운 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 클래스 인스턴스를 초기화합니다.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


`pbz4`/`bv41` 압축 블록 각각의 크기를 가져옵니다.

값: 기본값은 4 MiB입니다.

**Returns:**
int - 각 압축된 `pbz4`/`bv41` 블록의 크기.
