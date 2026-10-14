---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP for Java API 참조"
description: "Data Descriptor 존재에 대한 옵션."
type: docs
weight: 171
url: /ko/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Data Descriptor 존재에 대한 옵션.
## 필드

| 필드 | 설명 |
| --- | --- |
| [Always](#Always) | Data Descriptor는 모든 zip 항목에 항상 존재합니다. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor는 파일 데이터가 있는 항목에만 존재하고, 디렉터리에는 생략됩니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor는 모든 zip 항목에 항상 존재합니다.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor는 파일 데이터가 있는 항목에만 존재하고, 디렉터리에는 생략됩니다. 이 옵션의 사용은 권장되지 않습니다.

암호화되지 않은 아카이브에만 적용할 수 있습니다.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
