---
title: "ZArchiveSaveOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per Zarchive."
type: docs
weight: 155
url: /it/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

Impostazioni per Zarchive.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento che viene sollevato quando una porzione di stream grezzo è compressa |

