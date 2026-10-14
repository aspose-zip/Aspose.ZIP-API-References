---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Speichern eines bzip2-Archivs."
type: docs
weight: 43
url: /de/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Optionen zum Speichern eines bzip2-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Initialisiert eine neue Instanz der [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions)-Klasse. |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Initialisiert eine neue Instanz der [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions)-Klasse mit der Standard-Blockgröße von 9 Hundert Kilobyte. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blockgröße in Hunderten von Kilobyte. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [getCompressionThreads()](#getCompressionThreads--) | Liefert die Anzahl der Komprimierungs-Threads. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Setzt die Anzahl der Komprimierungs-Threads. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Initialisiert eine neue Instanz der [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions)-Klasse.

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


Blockgröße in Hunderten von Kilobyte.

**Returns:**
int - Blockgröße in Hunderten von Kilobyte
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird.

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

Dieses Ereignis wird nicht ausgelöst, wenn in mehrthreadigem Modus komprimiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Setzt die Anzahl der Komprimierungs-Threads. Wenn der Wert größer als 1 ist, wird eine mehrthreadige Komprimierung verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Komprimierungs-Thread-Anzahl. |

