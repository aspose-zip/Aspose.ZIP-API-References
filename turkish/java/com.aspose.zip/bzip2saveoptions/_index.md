---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "bzip2 arşivi kaydetmek için seçenekler."
type: docs
weight: 43
url: /tr/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

bzip2 arşivi kaydetmek için seçenekler.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Yeni bir [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) sınıfının örneğini başlatır. |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Varsayılan blok boyutu 9 yüz kilobyte olan bir [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blok boyutu yüz kilobyte cinsinden. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır. |
| [getCompressionThreads()](#getCompressionThreads--) | Sıkıştırma iş parçacığı sayısını alır. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı ayarlar. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sıkıştırma iş parçacığı sayısını ayarlar. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Yeni bir [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) sınıfının örneğini başlatır.

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


Blok boyutu yüz kilobyte cinsinden.

**Returns:**
int - blok boyutu yüz kilobyte cinsinden
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır.

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

Bu olay çok iş parçacıklı modda sıkıştırma yapıldığında tetiklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olay |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sıkıştırma iş parçacığı sayısını ayarlar. Değer 1'den büyükse, çok iş parçacıklı sıkıştırma kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sıkıştırma iş parçacığı sayısı. |

