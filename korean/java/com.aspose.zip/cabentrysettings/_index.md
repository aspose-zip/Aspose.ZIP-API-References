---
title: "CabEntrySettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "CAB 항목이 작성되는 방식을 제어하는 설정."
type: docs
weight: 47
url: /ko/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

CAB 항목이 작성되는 방식을 제어하는 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | 특정 압축 프로파일로 설정을 초기화합니다. |
| [CabEntrySettings()](#CabEntrySettings--) | 기본 MSZip 압축으로 설정을 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | 항목에 적용된 압축 구성을 가져옵니다. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


특정 압축 프로파일로 설정을 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | 사용할 압축 설정. |

다음 중 하나일 수 있습니다: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


기본 MSZip 압축으로 설정을 초기화합니다.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


항목에 적용된 압축 구성을 가져옵니다.

다음 중 하나일 수 있습니다:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
