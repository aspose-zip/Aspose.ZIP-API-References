---
title: "LzxLoadOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "압축된 파일에서 아카이브를 로드할 때 사용하는 옵션."
type: docs
weight: 91
url: /ko/java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

압축된 파일에서 아카이브를 로드할 때 사용하는 옵션.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다. |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다.

일정 시간 후에 ISO 아카이브 추출을 취소합니다.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzxLoadOptions options = new LzxLoadOptions();
options.setCancellationFlag(cf);
try (LzxArchive a = new LzxArchive("big.lzx", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

