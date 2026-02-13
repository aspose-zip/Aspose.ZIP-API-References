---
title: LzipLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for loading .
type: docs
weight: 68
url: /java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

Options for loading [LzipArchive](../../com.aspose.zip/lziparchive).

In the .NET Framework 4.0 and above, can be used to cancel extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel lzip archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         LzipLoadOptions options = new LzipLoadOptions();
         options.setCancellationFlag(cf);
         try (LzipArchive a = new LzipArchive("big.lz", options)) {
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

