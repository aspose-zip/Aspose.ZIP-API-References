---
title: "AlzArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een ALZ-archiefbestand voor."
type: docs
weight: 11
url: /nl/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Stelt een ALZ-archiefbestand voor. Gebruik deze klasse om ALZ-archieven te inspecteren en te extraheren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Initialiseert een ALZ-archief vanuit een stream. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Initialiseert een ALZ-archief vanuit een stream met de meegeleverde laadopties. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Initialiseert een ALZ-archief vanaf een bestandspad. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Initialiseert een ALZ-archief vanaf een bestandspad met de meegeleverde laadopties. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | Vrijgeeft bronnen die door dit archief worden vastgehouden. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden en mappen naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt de items op die dit archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op via de algemene archiefinterface. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Initialiseert een ALZ-archief vanuit een stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | ALZ-archiefstream; deze moet lezen en zoeken ondersteunen |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Initialiseert een ALZ-archief vanuit een stream met de meegeleverde laadopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | ALZ-archiefstream; deze moet lezen en zoeken ondersteunen |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opties gebruikt om het archief te laden |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Initialiseert een ALZ-archief vanaf een bestandspad.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | pad naar een ALZ-archief |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Initialiseert een ALZ-archief vanaf een bestandspad met de meegeleverde laadopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | pad naar een ALZ-archief |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opties gebruikt om het archief te laden |

### close() {#close--}
```
public void close()
```


Vrijgeeft bronnen die door dit archief worden vastgehouden.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert alle bestanden en mappen naar de opgegeven map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | java.lang.String | doelmap; deze wordt gemaakt wanneer nodig |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Haalt de items op die dit archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - onveranderlijke lijst van ALZ-items
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op via de algemene archiefinterface.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - archiefitems
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
