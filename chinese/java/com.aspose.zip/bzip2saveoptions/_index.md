---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "保存 bzip2 存档的选项。"
type: docs
weight: 43
url: /zh/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

保存 bzip2 存档的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | 初始化一个新的 [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) 类的实例。 |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | 使用默认块大小（等于 9 百千字节）初始化一个新的 [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 块大小，以百千字节为单位。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 获取在原始流的一部分被压缩时触发的事件。 |
| [getCompressionThreads()](#getCompressionThreads--) | 获取压缩线程数。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在原始流的一部分被压缩时触发的事件。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 设置压缩线程数。 |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


初始化一个新的 [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) 类的实例。

```

``````

try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
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


块大小，以百千字节为单位。

**Returns:**
int - 块大小，以百千字节为单位
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


获取在原始流的一部分被压缩时触发的事件。

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

在多线程模式下压缩时，此事件不会被触发。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 当原始流的一部分被压缩时触发的事件 |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


设置压缩线程数。如果该值大于 1，将使用多线程压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 压缩线程数。 |

