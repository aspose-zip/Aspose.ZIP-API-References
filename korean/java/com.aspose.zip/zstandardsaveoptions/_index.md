---
title: "ZstandardSaveOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZStandard 아카이브에 대한 설정입니다."
type: docs
weight: 159
url: /ko/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

ZStandard 아카이브에 대한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 설정합니다. |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다.

```

``````

File source = new File("huge.bin");
ZstandardSaveOptions settings = new ZstandardSaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     ZstandardSaveOptions settings = new ZstandardSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 원시 스트림의 일부가 압축될 때 발생하는 이벤트입니다. |

