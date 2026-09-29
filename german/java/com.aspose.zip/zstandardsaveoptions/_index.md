---
title: "ZstandardSaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für das ZStandard-Archiv."
type: docs
weight: 159
url: /de/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

Einstellungen für das ZStandard-Archiv.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird |

