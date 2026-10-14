---
title: "ZArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für Zarchive."
type: docs
weight: 155
url: /de/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

Einstellungen für Zarchive.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird.

```

``````

File source = new File("huge.bin");
ZArchiveSaveOptions settings = new ZArchiveSaveOptions();
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
     ZArchiveSaveOptions settings = new ZArchiveSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird |

