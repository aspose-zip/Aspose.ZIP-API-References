---
title: WimLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which archive is loaded from a compressed file.
type: docs
weight: 109
url: /java/com.aspose.zip/wimloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class WimLoadOptions
```

Options with which archive is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [WimLoadOptions()](#WimLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
### WimLoadOptions() {#WimLoadOptions--}
```
public WimLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel WIM archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         WimLoadOptions options = new WimLoadOptions();
         options.setCancellationFlag(cf);
         try (WimArchive a = new WimArchive("big.wim", options)) {
             try {
                 StreamSupport.stream(a.getImages().get(0).getAllEntries().spliterator(), false)
                              .filter(entry -> entry instanceof WimFileEntry)
                              .map(entry -> (WimFileEntry) entry)
                              .findFirst().ifPresent(entry -> entry.extract("data.bin"));
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

