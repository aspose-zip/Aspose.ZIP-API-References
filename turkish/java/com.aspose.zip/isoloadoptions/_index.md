---
title: "IsoLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Sıkıştırılmış bir dosyadan  yüklenirken kullanılan seçenekler."
type: docs
weight: 73
url: /tr/java/com.aspose.zip/isoloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class IsoLoadOptions
```

Sıkıştırılmış bir dosyadan [IsoArchive](../../com.aspose.zip/isoarchive) yüklenirken kullanılan seçenekler. Çıkarma sırasında tetiklenen olayı içerir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [IsoLoadOptions()](#IsoLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Bazı baytlar çıkarıldığında tetiklenen bir olayı alır. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Bazı baytlar çıkarıldığında tetiklenen bir olayı ayarlar. |
### IsoLoadOptions() {#IsoLoadOptions--}
```
public IsoLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Bazı baytlar çıkarıldığında tetiklenen bir olayı alır.

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

Cancellation çoğunlukla bazı verilerin çıkarılmamasına neden olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | çıkarma işlemini iptal etmek için kullanılan bir cancellation flag. |

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


Bazı baytlar çıkarıldığında tetiklenen bir olayı ayarlar.

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

