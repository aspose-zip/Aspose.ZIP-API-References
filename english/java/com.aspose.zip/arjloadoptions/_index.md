---
title: ArjLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which archive is loaded from a compressed file.
type: docs
weight: 23
url: /java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Options with which archive is loaded from a compressed file.

In the .NET Framework 4.0 and above, can be used to cancel extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ARJ archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ArjLoadOptions options = new ArjLoadOptions();
         options.setCancellationFlag(cf);
         try (ArjArchive a = new ArjArchive("big.arj", options)) {
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

