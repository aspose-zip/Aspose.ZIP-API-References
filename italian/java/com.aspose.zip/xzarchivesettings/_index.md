---
title: "XzArchiveSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "La classe contiene un insieme di impostazioni per un archivio xz particolare."
type: docs
weight: 147
url: /it/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

La classe contiene un insieme di impostazioni per un archivio xz particolare.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Inizializza una nuova istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) utilizzando la compressione LZMA2 singola. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Inizializza una nuova istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con parametri personalizzati. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Restituisce il conteggio dei thread di compressione. |
| [getFastSpeed()](#getFastSpeed--) | Ottiene l'istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con dimensione del dizionario pari a 1 megabyte nel filtro LZMA2, dimensione del blocco pari a 4 megabyte e checksum CRC32. |
| [getFastestSpeed()](#getFastestSpeed--) | Ottiene l'istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con dimensione del dizionario pari a 65536 byte nel filtro LZMA2, dimensione del blocco pari a 1 megabyte e checksum CRC32. |
| [getHighCompression()](#getHighCompression--) | Ottiene l'istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con dimensione del dizionario pari a 32 megabyte nel filtro LZMA2, dimensione del blocco pari a 128 megabyte e checksum CRC32. |
| [getMaximumCompression()](#getMaximumCompression--) | Ottiene l'istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con dimensione del dizionario pari a 64 megabyte nel filtro LZMA2, dimensione del blocco pari a 256 megabyte e checksum CRC32. |
| [getNormal()](#getNormal--) | Ottiene l'istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con dimensione del dizionario pari a 16 megabyte nel filtro LZMA2, dimensione del blocco pari a 64 megabyte e checksum CRC32. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Imposta il conteggio dei thread di compressione. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Inizializza una nuova istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) utilizzando la compressione LZMA2 singola.

Il dizionario predefinito nel filtro LZMA2 ha dimensione pari a 16 megabyte, la dimensione del blocco predefinita è pari a 64 megabyte, il tipo di checksum predefinito è CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Inizializza una nuova istanza della classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) con parametri personalizzati.

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save(xzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [XzFilterSettings\[\]](../../com.aspose.zip/xzfiltersettings) | filters (compressors) to be sequentially applied to create [XzArchive](../../com.aspose.zip/xzarchive). It can be either single [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) or pair of [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) and [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) |
| blockSize | long | size xz archive block |
| checkType | [XzCheckType](../../com.aspose.zip/xzchecktype) | type of checksum calculation for uncompressed data |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### getFastSpeed() {#getFastSpeed--}
```
public static XzArchiveSettings getFastSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fast speed
### getFastestSpeed() {#getFastestSpeed--}
```
public static XzArchiveSettings getFastestSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fastest speed
### getHighCompression() {#getHighCompression--}
```
public static XzArchiveSettings getHighCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the high compression
### getMaximumCompression() {#getMaximumCompression--}
```
public static XzArchiveSettings getMaximumCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the maximum compression
### getNormal() {#getNormal--}
```
public static XzArchiveSettings getNormal()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with normal parameters
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores |

