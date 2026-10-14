---
title: "ZstandardSaveOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour l'archive ZStandard."
type: docs
weight: 159
url: /fr/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

Paramètres pour l'archive ZStandard.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée.

```

``````

File source = new File(\"huge.bin\");
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
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un événement qui est déclenché lorsqu'une partie du flux brut est compressée |

