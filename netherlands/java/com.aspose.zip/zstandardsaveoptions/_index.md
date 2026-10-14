---
title: "ZstandardSaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor ZStandard-archief."
type: docs
weight: 159
url: /nl/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

Instellingen voor ZStandard-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream wordt gecomprimeerd |

