---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "로드 옵션."
type: docs
weight: 70
url: /ko/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

로드 옵션 [GzipArchive](../../com.aspose.zip/gziparchive).

.NET Framework 4.0 이상에서는 추출을 취소하는 데 사용할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | 스트림 헤더를 구문 분석하여 속성(이름 포함)을 확인할지 여부를 나타내는 값을 가져옵니다. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | 스트림 헤더를 구문 분석하여 속성(이름 포함)을 확인할지 여부를 나타내는 값을 설정합니다. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


스트림 헤더를 구문 분석하여 속성(이름 포함)을 확인할지 여부를 가져옵니다. 탐색 가능한 스트림에만 의미가 있습니다.

**Returns:**
boolean - 스트림 헤더를 구문 분석하여 속성(이름 포함)을 확인할지 여부를 나타내는 값.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다.

특정 시간 후에 gzip 아카이브 추출을 취소합니다.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("추출이 60초 후에 취소되었습니다");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

