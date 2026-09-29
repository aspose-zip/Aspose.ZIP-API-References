---
title: "IsoLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры, с помощью которых  загружается из сжатого файла."
type: docs
weight: 73
url: /ru/java/com.aspose.zip/isoloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class IsoLoadOptions
```

Параметры, с помощью которых [IsoArchive](../../com.aspose.zip/isoarchive) загружается из сжатого файла. Содержит событие, вызываемое при извлечении.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [IsoLoadOptions()](#IsoLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Получает событие, которое вызывается, когда некоторые байты извлечены. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда некоторые байты извлечены. |
### IsoLoadOptions() {#IsoLoadOptions--}
```
public IsoLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Получает событие, которое вызывается, когда некоторые байты извлечены.

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive("archive.iso", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ISO archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         IsoLoadOptions options = new IsoLoadOptions();
         options.setCancellationFlag(cf);
         try (IsoArchive a = new IsoArchive("big.iso", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

Отмена обычно приводит к тому, что некоторые данные не извлекаются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | Флаг отмены, используемый для прерывания операции извлечения. |

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


Устанавливает событие, которое вызывается, когда некоторые байты извлечены.

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive("archive.iso", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

