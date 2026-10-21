---
title: "AlzArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en ALZ-arkivfil."
type: docs
weight: 11
url: /sv/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Representerar en ALZ-arkivfil. Använd den här klassen för att inspektera och extrahera ALZ-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Initierar ett ALZ-arkiv från en ström. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Initierar ett ALZ-arkiv från en ström med de medföljande laddningsalternativen. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Initierar ett ALZ-arkiv från en filsökväg. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Initierar ett ALZ-arkiv från en filsökväg med de medföljande laddningsalternativen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | Frigör resurser som hålls av detta arkiv. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla filer och kataloger till den angivna katalogen. |
| [getEntries()](#getEntries--) | Hämtar posterna som utgör detta arkiv. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster via det gemensamma arkivgränssnittet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Initierar ett ALZ-arkiv från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | ALZ-arkivström; den måste stödja läsning och sökning |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Initierar ett ALZ-arkiv från en ström med de medföljande laddningsalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | ALZ-arkivström; den måste stödja läsning och sökning |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | alternativ som används för att ladda arkivet |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Initierar ett ALZ-arkiv från en filsökväg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | sökväg till ett ALZ-arkiv |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Initierar ett ALZ-arkiv från en filsökväg med de medföljande laddningsalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | sökväg till ett ALZ-arkiv |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | alternativ som används för att ladda arkivet |

### close() {#close--}
```
public void close()
```


Frigör resurser som hålls av detta arkiv.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar alla filer och kataloger till den angivna katalogen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | java.lang.String | destinationskatalog; den skapas vid behov |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Hämtar posterna som utgör detta arkiv.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - oföränderlig lista med ALZ-poster
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster via det gemensamma arkivgränssnittet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - arkivposter
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Hämtar arkivformatet.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
