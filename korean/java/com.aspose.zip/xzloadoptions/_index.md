---
title: "XzLoadOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "로드 옵션."
type: docs
weight: 152
url: /ko/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

로드를 위한 옵션 [XzArchive](../../com.aspose.zip/xzarchive).

.NET Framework 4.0 이상에서는 추출을 취소하는 데 사용할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다.

일정 시간 후에 lzip 아카이브 추출을 취소합니다.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

