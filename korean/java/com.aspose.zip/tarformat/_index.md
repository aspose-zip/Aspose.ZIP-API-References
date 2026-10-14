---
title: "TarFormat"
second_title: "Aspose.ZIP for Java API 참조"
description: "지원되는 형식의 열거형입니다."
type: docs
weight: 169
url: /ko/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

[TarArchive](../../com.aspose.zip/tararchive)의 지원되는 형식 열거형입니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [Gnu](#Gnu) | GNU tar는 POSIX.1의 초기 초안에 기반합니다. |
| [Pax](#Pax) | 포맷은 POSIX.1-2001 표준에 정의됩니다. |
| [UsTar](#UsTar) | 포맷은 v7 포맷의 헤더 블록을 확장합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar는 POSIX.1의 초기 초안에 기반합니다. 이 포맷은 많은 Linux 시스템에서 기본 tar 포맷으로 구현됩니다.

### Pax {#Pax}
```
public static final TarFormat Pax
```


포맷은 POSIX.1-2001 표준에 정의됩니다.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


포맷은 v7 포맷의 헤더 블록을 확장합니다. Windows용 많은 유틸리티에서 널리 사용되고 지원됩니다.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
