---
title: "Bzip2SaveOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para guardar un archivo bzip2."
type: docs
weight: 43
url: /es/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Opciones para guardar un archivo bzip2.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Inicializa una nueva instancia de la clase [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions). |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Inicializa una nueva instancia de la clase [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) con el tamaño de bloque predeterminado, igual a 9 cientos de kilobytes. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Tamaño de bloque en cientos de kilobytes. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [getCompressionThreads()](#getCompressionThreads--) | Obtiene el recuento de hilos de compresión. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Establece el recuento de hilos de compresión. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Inicializa una nueva instancia de la clase [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions).

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


Tamaño de bloque en cientos de kilobytes.

**Returns:**
int - tamaño de bloque en cientos de kilobytes
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar.

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

Este evento no se activará al comprimir en modo multihilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento que se genera cuando una porción del flujo sin procesar se comprime. |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Establece el recuento de hilos de compresión. Si el valor es mayor que 1, se utilizará compresión multihilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | recuento de hilos de compresión. |

