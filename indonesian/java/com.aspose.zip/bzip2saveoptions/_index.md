---
title: "Bzip2SaveOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk menyimpan arsip bzip2."
type: docs
weight: 43
url: /id/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Opsi untuk menyimpan arsip bzip2.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Menginisialisasi sebuah instance baru dari kelas [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions). |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Menginisialisasi sebuah instance baru dari kelas [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) dengan ukuran blok default, yaitu 9 ratus kilobyte. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ukuran blok dalam ratus kilobyte. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [getCompressionThreads()](#getCompressionThreads--) | Mendapatkan jumlah thread kompresi. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Mengatur jumlah thread kompresi. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Menginisialisasi sebuah instance baru dari kelas [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions).

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


Ukuran blok dalam ratus kilobyte.

**Returns:**
int - ukuran blok dalam ratus kilobyte
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi.

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

Peristiwa ini tidak akan dipicu saat melakukan kompresi dalam mode multithread.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | sebuah event yang dipicu ketika sebagian aliran mentah dikompresi |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Mengatur jumlah thread kompresi. Jika nilai lebih besar dari 1, kompresi multithread akan digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah thread kompresi. |

