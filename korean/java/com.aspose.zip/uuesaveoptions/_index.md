---
title: "UueSaveOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "uuencoded 파일 저장 옵션."
type: docs
weight: 129
url: /ko/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

uuencoded 파일 저장 옵션.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | 사용자가 제공한 파일 이름과 새 줄을 사용하여 옵션을 초기화합니다. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | 사용자가 제공한 파일 이름과 기본 새 줄을 사용하여 옵션을 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFileName()](#getFileName--) | 디코딩된 데이터를 재생성할 때 사용할 파일 이름을 가져옵니다. |
| [getNewLine()](#getNewLine--) | 각 줄을 종료하는 문자를 가져옵니다. 일반적으로 "\\n" 또는 "\\r\\n"입니다. |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | 파일의 Unix 파일 권한을 가져옵니다. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | 파일의 Unix 파일 권한을 설정합니다. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


사용자가 제공한 파일 이름과 새 줄을 사용하여 옵션을 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 디코딩된 데이터를 재생성할 때 사용할 파일 이름 |
| newLine | java.lang.String | 각 행을 종료하는 문자 |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


사용자가 제공한 파일 이름과 기본 새 줄을 사용하여 옵션을 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 디코딩된 데이터를 재생성할 때 사용할 파일 이름 |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


디코딩된 데이터를 재생성할 때 사용할 파일 이름을 가져옵니다.

**Returns:**
java.lang.String - 디코딩된 데이터를 재생성할 때 사용할 파일 이름
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


각 줄을 종료하는 문자를 가져옵니다. 일반적으로 "\\n" 또는 "\\r\\n"입니다.

**Returns:**
java.lang.String - 각 행을 종료하는 문자, 일반적으로 "\n" 또는 "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


파일의 Unix 파일 권한을 가져옵니다.

기본값은 644입니다.

**Returns:**
java.lang.String - 파일의 Unix 파일 권한
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


파일의 Unix 파일 권한을 설정합니다.

기본값은 644입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 파일의 Unix 파일 권한 |

