---
title: "ZstandardSaveOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per l'archivio ZStandard."
type: docs
weight: 159
url: /it/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

Impostazioni per l'archivio ZStandard.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento che viene sollevato quando una porzione di stream grezzo è compressa |

