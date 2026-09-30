---
title: "ZArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Zarchive için ayarlar."
type: docs
weight: 155
url: /tr/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

Zarchive için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı ayarlar. |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olay |

