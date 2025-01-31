---
title: Bzip2SaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving a bzip2 archive.
type: docs
weight: 26
url: /java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Options for saving a bzip2 archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class. |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class with default block size, equals to 9 hundred of kilobytes. |
## Methods

| Method | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Block size in hundreds of kilobytes. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gets an event that is raised when a portion of raw stream compressed. |
| [getCompressionThreads()](#getCompressionThreads--) | Gets compression thread count. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when a portion of raw stream compressed. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sets compression thread count. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class.

```

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


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

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


Gets compression thread count. If the value greater than 1, multithreading compression will be used.

**Returns:**
int - Compression thread count.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

     File source = new File("huge.bin");
     Bzip2SaveOptions settings = new Bzip2SaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```

This event won't be raised when compressing in multithreaded mode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Compression thread count. |

