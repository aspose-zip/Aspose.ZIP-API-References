---
title: "Bzip2SaveOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры сохранения архива bzip2."
type: docs
weight: 43
url: /ru/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Параметры сохранения архива bzip2.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Инициализирует новый экземпляр класса [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions). |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Инициализирует новый экземпляр класса [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) с размером блока по умолчанию, равным 9 сотням килобайт. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Размер блока в сотнях килобайт. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Получает событие, которое вызывается, когда часть необработанного потока сжата. |
| [getCompressionThreads()](#getCompressionThreads--) | Получает количество потоков сжатия. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда часть необработанного потока сжата. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Устанавливает количество потоков сжатия. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Инициализирует новый экземпляр класса [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions).

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


Размер блока в сотнях килобайт.

**Returns:**
int — размер блока в сотнях килобайт
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Получает событие, которое вызывается, когда часть необработанного потока сжата.

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

Это событие не будет вызываться при сжатии в многопоточном режиме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | событие, которое вызывается, когда часть необработанного потока сжата |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Устанавливает количество потоков сжатия. Если значение больше 1, будет использоваться многопоточное сжатие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int | количество потоков сжатия. |

