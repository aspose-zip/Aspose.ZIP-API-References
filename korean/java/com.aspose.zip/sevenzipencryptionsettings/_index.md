---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "여러 7z 암호화 방법에 대한 설정의 기본 클래스."
type: docs
weight: 112
url: /ko/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

여러 7z 암호화 방법에 대한 설정의 기본 클래스.

AES-256는 7z 아카이브에 사용할 수 있는 유일한 암호화 방법입니다. 따라서 [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings)는 유일한 구현입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | 헤더 암호화를 나타내는 값을 가져옵니다. |
| [getPassword()](#getPassword--) | 암호화 또는 복호화를 위한 비밀번호를 가져옵니다. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | 헤더 암호화를 나타내는 값을 설정합니다. |
| [setPassword(String value)](#setPassword-java.lang.String-) | 암호화 또는 복호화를 위한 비밀번호를 설정합니다. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


헤더 암호화를 나타내는 값을 가져옵니다.

이 설정은 7-Zip 도구의 `-mhe=on` 스위치와 동일합니다. 현재 헤더 압축과 호환되지 않습니다.

**Returns:**
boolean - 헤더 암호화를 나타내는 값
### getPassword() {#getPassword--}
```
public final String getPassword()
```


암호화 또는 복호화를 위한 비밀번호를 가져옵니다.

**Returns:**
java.lang.String - 암호화 또는 복호화를 위한 비밀번호
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


헤더 암호화를 나타내는 값을 설정합니다.

이 설정은 7-Zip 도구의 `-mhe=on` 스위치와 동일합니다. 현재 헤더 압축과 호환되지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 헤더 암호화를 나타내는 값 |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


암호화 또는 복호화를 위한 비밀번호를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 암호화 또는 복호화를 위한 비밀번호 |

