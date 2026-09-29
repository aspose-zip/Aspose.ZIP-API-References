---
title: "ZArchiveSaveOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk Zarchive."
type: docs
weight: 155
url: /id/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

Pengaturan untuk Zarchive.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi.

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | sebuah event yang dipicu ketika sebagian aliran mentah dikompresi |

