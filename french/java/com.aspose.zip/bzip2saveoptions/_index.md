---
title: "Bzip2SaveOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour enregistrer une archive bzip2."
type: docs
weight: 43
url: /fr/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Options pour enregistrer une archive bzip2.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Initialise une nouvelle instance de la classe [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions). |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Initialise une nouvelle instance de la classe [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) avec une taille de bloc par défaut, égale à 9 centaines de kilo-octets. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Taille du bloc en centaines de kilo-octets. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [getCompressionThreads()](#getCompressionThreads--) | Obtient le nombre de threads de compression. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Définit le nombre de threads de compression. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Initialise une nouvelle instance de la classe [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions).

```

``````

try (FileOutputStream result = new FileOutputStream(\"archive.bz2\")) {
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


Taille du bloc en centaines de kilo-octets.

**Returns:**
int - taille du bloc en centaines de kilo-octets
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée.

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

Cet événement ne sera pas déclenché lors de la compression en mode multithread.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un événement qui est déclenché lorsqu'une partie du flux brut est compressée |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Définit le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | nombre de threads de compression. |

