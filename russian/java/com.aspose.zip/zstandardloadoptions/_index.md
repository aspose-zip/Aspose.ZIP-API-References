---
title: "ZstandardLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры, с помощью которых  загружается из сжатого файла."
type: docs
weight: 158
url: /ru/java/com.aspose.zip/zstandardloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardLoadOptions
```

Параметры, с помощью которых [ZstandardArchive](../../com.aspose.zip/zstandardarchive) загружается из сжатого файла. Содержит событие, возникающее при извлечении.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ZstandardLoadOptions()](#ZstandardLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Получает событие, которое вызывается, когда некоторые байты извлечены. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда некоторые байты извлечены. |
### ZstandardLoadOptions() {#ZstandardLoadOptions--}
```
public ZstandardLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Получает событие, которое вызывается, когда некоторые байты извлечены.

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Zstandard archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZstandardLoadOptions options = new ZstandardLoadOptions();
         options.setCancellationFlag(cf);
         try (ZstandardArchive a = new ZstandardArchive("big.zstd", options)) {
             try {
                 a.extract("data.bin");
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

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Устанавливает событие, которое вызывается, когда некоторые байты извлечены.

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

