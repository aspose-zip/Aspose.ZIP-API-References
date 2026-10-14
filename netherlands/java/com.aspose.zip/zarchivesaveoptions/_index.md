---
title: "ZArchiveSaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor Zarchive."
type: docs
weight: 155
url: /nl/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

Instellingen voor Zarchive.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd.

```

``````

File source = new File(\"huge.bin\");
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream wordt gecomprimeerd |

