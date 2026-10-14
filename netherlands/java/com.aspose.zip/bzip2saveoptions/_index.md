---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het opslaan van een bzip2-archief."
type: docs
weight: 43
url: /nl/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Opties voor het opslaan van een bzip2-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Initialiseert een nieuw exemplaar van de klasse [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class. |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Initialiseert een nieuw exemplaar van de klasse [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class met de standaard blokgrootte, gelijk aan 9 honderd kilobytes. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blokgrootte in honderden kilobytes. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [getCompressionThreads()](#getCompressionThreads--) | Haalt het aantal compressiedraden op. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Stelt het aantal compressiedraden in. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Initialiseert een nieuw exemplaar van de klasse [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class.

```

``````

try (FileOutputStream result = new FileOutputStream(\"archive.bz2\")) {
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


Blokgrootte in honderden kilobytes.

**Returns:**
int - blokgrootte in honderden kilobytes
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd.

```

``````

File source = new File(\"huge.bin\");
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

Dit evenement wordt niet getriggerd bij compressie in multithread-modus.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream wordt gecomprimeerd |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Stelt het aantal compressiedraden in. Als de waarde groter is dan 1, wordt multithread-compressie gebruikt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | aantal compressiedraden. |

