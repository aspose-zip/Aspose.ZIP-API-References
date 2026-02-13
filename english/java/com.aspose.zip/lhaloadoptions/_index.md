---
title: LhaLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which archive is loaded from a compressed file.
type: docs
weight: 61
url: /java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

Options with which archive is loaded from a compressed file.

In the .NET Framework 4.0 and above, can be used to cancel extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel LHA archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         LhaLoadOptions options = new LhaLoadOptions();
         options.setCancellationFlag(cf);
         try (LhaArchive a = new LhaArchive("big.lha", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
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

