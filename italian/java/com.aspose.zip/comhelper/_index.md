---
title: "ComHelper"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Fornisce metodi per i client COM per caricare archivi in Aspose.Zip."
type: docs
weight: 55
url: /it/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Fornisce metodi per i client COM per caricare archivi in Aspose.Zip.

Utilizza la classe **ComHelper** per caricare un archivio da un file o da uno stream. Classi specifiche forniscono un costruttore predefinito per creare un nuovo archivio e forniscono anche costruttori sovraccaricati per caricare un archivio da un file o da uno stream. Se utilizzi **Aspose.Zip** da un'applicazione .NET, puoi usare tutti i costruttori dell'archivio direttamente, ma se utilizzi **Aspose.Zip** da un'applicazione COM, è disponibile solo il costruttore predefinito dell'archivio.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ComHelper()](#ComHelper--) | Inizializza una nuova istanza di questa classe. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Consente a un'applicazione COM di caricare un archivio bzip2 da uno stream. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Consente a un'applicazione COM di caricare un archivio bzip2 da un file. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Consente a un'applicazione COM di caricare un archivio gzip da uno stream. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Consente a un'applicazione COM di caricare un archivio gzip da un file. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Consente a un'applicazione COM di caricare un archivio rar da uno stream. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Consente a un'applicazione COM di caricare un archivio rar da un file. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Consente a un'applicazione COM di caricare un archivio ZIP da uno stream. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Consente a un'applicazione COM di caricare un archivio ZIP da un file. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Inizializza una nuova istanza di questa classe.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Consente a un'applicazione COM di caricare un archivio bzip2 da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Un oggetto stream .NET che contiene l'archivio da caricare. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Consente a un'applicazione COM di caricare un archivio bzip2 da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Nome file dell'archivio da caricare. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Consente a un'applicazione COM di caricare un archivio gzip da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Un oggetto stream .NET che contiene l'archivio da caricare. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Consente a un'applicazione COM di caricare un archivio gzip da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Nome file dell'archivio da caricare. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Consente a un'applicazione COM di caricare un archivio rar da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Un oggetto stream .NET che contiene l'archivio da caricare. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Consente a un'applicazione COM di caricare un archivio rar da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Nome file dell'archivio da caricare. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Consente a un'applicazione COM di caricare un archivio ZIP da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Un oggetto stream .NET che contiene l'archivio da caricare. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Consente a un'applicazione COM di caricare un archivio ZIP da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Nome file dell'archivio da caricare. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
