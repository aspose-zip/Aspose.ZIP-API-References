---
title: "Bzip2LoadOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "로드 옵션."
type: docs
weight: 42
url: /ko/java/com.aspose.zip/bzip2loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2LoadOptions
```

[Bzip2Archive](../../com.aspose.zip/bzip2archive)를 로드하기 위한 옵션입니다. 추출 시 발생하는 이벤트를 포함합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Bzip2LoadOptions()](#Bzip2LoadOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | 일부 바이트가 추출될 때 발생하는 이벤트를 가져옵니다. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 추출 작업을 취소하는 데 사용되는 취소 플래그를 설정합니다. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 일부 바이트가 추출될 때 발생하는 이벤트를 설정합니다. |
### Bzip2LoadOptions() {#Bzip2LoadOptions--}
```
public Bzip2LoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


일부 바이트가 추출될 때 발생하는 이벤트를 가져옵니다.

```

``````

int[] percent = { 0 };
long originalFileLength = 10_000_000;

Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
});
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Bzip2 archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         Bzip2LoadOptions options = new Bzip2LoadOptions();
         options.setCancellationFlag(cf);
         try (Bzip2Archive a = new Bzip2Archive("big.bz2", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

취소는 대부분 일부 데이터가 추출되지 않는 결과를 초래합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 추출 작업을 취소하는 데 사용되는 취소 플래그. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


일부 바이트가 추출될 때 발생하는 이벤트를 설정합니다.

```

``````

int[] percent = { 0 };
long originalFileLength = 10_000_000;

Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
});
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

