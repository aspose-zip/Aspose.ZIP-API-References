---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "bzip2 아카이브를 저장하기 위한 옵션."
type: docs
weight: 43
url: /ko/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

bzip2 아카이브를 저장하기 위한 옵션.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | 새로운 [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) 클래스의 인스턴스를 초기화합니다. |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | 기본 블록 크기인 9백 킬로바이트로 새로운 [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) 클래스의 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 블록 크기(백 킬로바이트 단위). |
| [getCompressionProgressed()](#getCompressionProgressed--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다. |
| [getCompressionThreads()](#getCompressionThreads--) | 압축 스레드 수를 가져옵니다. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 설정합니다. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 압축 스레드 수를 설정합니다. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


새로운 [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) 클래스의 인스턴스를 초기화합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(\"data.bin\");
archive.save(result, new Bzip2SaveOptions(9));
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2SaveOptions() {#Bzip2SaveOptions--}
```
public Bzip2SaveOptions()
```


Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
         try (Bzip2Archive archive = new Bzip2Archive()) {
             archive.setSource("data.bin");
             archive.save(result, new Bzip2SaveOptions());
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


블록 크기(백 킬로바이트 단위).

**Returns:**
int - 블록 크기(백 킬로바이트 단위)
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다.

```

``````

File source = new File("huge.bin");
Bzip2SaveOptions settings = new Bzip2SaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```

This event won't be raised when compressing in multithreaded mode.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     Bzip2SaveOptions settings = new Bzip2SaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```

이 이벤트는 다중 스레드 모드로 압축할 때 발생하지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 원시 스트림의 일부가 압축될 때 발생하는 이벤트입니다. |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


압축 스레드 수를 설정합니다. 값이 1보다 크면 다중 스레드 압축이 사용됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int | 압축 스레드 수. |

