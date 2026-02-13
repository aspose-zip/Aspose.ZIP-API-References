---
title: LzxLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which archive is loaded from a compressed file.
type: docs
weight: 74
url: /java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

Options with which archive is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ISO archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         LzxLoadOptions options = new LzxLoadOptions();
         options.setCancellationFlag(cf);
         try (LzxArchive a = new LzxArchive("big.lzx", options)) {
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

