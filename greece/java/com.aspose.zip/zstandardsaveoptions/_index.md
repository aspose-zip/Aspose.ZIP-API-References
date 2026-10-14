---
title: "ZstandardSaveOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για το αρχείο ZStandard."
type: docs
weight: 159
url: /el/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

Ρυθμίσεις για το αρχείο ZStandard.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται.

```

``````

File source = new File("huge.bin");
ZstandardSaveOptions settings = new ZstandardSaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     ZstandardSaveOptions settings = new ZstandardSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής |

