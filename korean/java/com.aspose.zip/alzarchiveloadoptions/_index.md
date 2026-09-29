---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "압축 파일에서 ALZ 아카이브를 로드할 때 사용되는 옵션입니다."
type: docs
weight: 12
url: /ko/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

압축 파일에서 ALZ 아카이브를 로드할 때 사용되는 옵션입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | 항목을 복호화하는 데 사용되는 비밀번호를 가져옵니다. |
| [getEncoding()](#getEncoding--) | 항목 이름에 사용되는 인코딩을 가져옵니다. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | ALZ 항목에 대한 체크섬 검증이 건너뛰어지는지 여부를 가져옵니다. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 추출을 취소하는 데 사용되는 취소 플래그를 설정합니다. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | 항목을 복호화하는 데 사용되는 비밀번호를 설정합니다. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 항목 이름에 사용되는 인코딩을 설정합니다. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | ALZ 항목에 대한 체크섬 검증을 건너뛰는지 여부를 설정합니다. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


항목을 복호화하는 데 사용되는 비밀번호를 가져옵니다.

**Returns:**
java.lang.String - 항목을 복호화하는 데 사용되는 비밀번호, 또는 설정되지 않은 경우 `null`
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


항목 이름에 사용되는 인코딩을 가져옵니다. 기본값은 한국어 Windows 코드 페이지 949(CP949)입니다. ALZ 아카이브는 역사적으로 파일 이름을 한국어 Windows ANSI 코드 페이지를 사용하여 저장합니다.

**Returns:**
java.nio.charset.Charset - 항목 이름에 사용되는 인코딩
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


ALZ 항목에 대한 체크섬 검증이 건너뛰어지는지 여부를 가져옵니다. 기본값은 `false`입니다.

**Returns:**
boolean - 체크섬 검증을 건너뛰는지 여부
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


추출을 취소하는 데 사용되는 취소 플래그를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 취소 플래그, 또는 취소를 비활성화하려면 `null` |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


항목을 복호화하는 데 사용되는 비밀번호를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 항목을 복호화하는 데 사용되는 비밀번호 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


항목 이름에 사용되는 인코딩을 설정합니다. ALZ 아카이브는 역사적으로 파일 이름을 한국어 Windows ANSI 코드 페이지를 사용하여 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.nio.charset.Charset | 항목 이름에 사용되는 인코딩 |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


ALZ 항목에 대한 체크섬 검증을 건너뛰는지 여부를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 체크섬 검증을 건너뛰는지 여부 |

