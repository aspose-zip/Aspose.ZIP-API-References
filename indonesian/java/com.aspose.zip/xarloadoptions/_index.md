---
title: "XarLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi dengan mana arsip XAR dimuat dari file terkompresi."
type: docs
weight: 142
url: /id/java/com.aspose.zip/xarloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XarLoadOptions
```

Opsi dengan mana arsip XAR dimuat dari file terkompresi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XarLoadOptions()](#XarLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Mendapatkan sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak. |
### XarLoadOptions() {#XarLoadOptions--}
```
public XarLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Mendapatkan sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak.

```

``````

XarLoadOptions loadOptions = new XarLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / ((XarFileEntry)sender).getLength());
});
XarArchive archive = new XarArchive("archive.xar", loadOptions);
 
```

Event sender is the [XarFileEntry](../../com.aspose.zip/xarfileentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel XAR archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         XarLoadOptions options = new XarLoadOptions();
         options.setCancellationFlag(cf);
         try (XarArchive a = new XarArchive("big.xar", options)) {
             try {
                 ((XarFileEntry) a.getEntries().get(0)).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

Pembatalan biasanya mengakibatkan sebagian data tidak diekstrak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | bendera pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


Mengatur sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak.

```

``````

XarLoadOptions loadOptions = new XarLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / ((XarFileEntry)sender).getLength());
});
XarArchive archive = new XarArchive("archive.xar", loadOptions);
 
```

Event sender is the [XarFileEntry](../../com.aspose.zip/xarfileentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

