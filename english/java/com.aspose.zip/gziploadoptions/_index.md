---
title: GzipLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for loading .
type: docs
weight: 48
url: /java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Options for loading [GzipArchive](../../com.aspose.zip/gziparchive).

In the .NET Framework 4.0 and above, can be used to cancel extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Gets the value indicating whether to parse stream header to figure out properties, including name. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Sets the value indicating whether to parse stream header to figure out properties, including name. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Gets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Returns:**
boolean - the value indicating whether to parse stream header to figure out properties, including name.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel gzip archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         GzipLoadOptions options = new GzipLoadOptions();
         options.setCancellationFlag(cf);
         try (GzipArchive a = new GzipArchive("big.gz", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

