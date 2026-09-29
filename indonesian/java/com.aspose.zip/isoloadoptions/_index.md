---
title: "IsoLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi dengan mana  dimuat dari file terkompresi."
type: docs
weight: 73
url: /id/java/com.aspose.zip/isoloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class IsoLoadOptions
```

Opsi dengan mana [IsoArchive](../../com.aspose.zip/isoarchive) dimuat dari berkas terkompresi. Berisi peristiwa yang dipicu saat ekstraksi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [IsoLoadOptions()](#IsoLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Mendapatkan sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak. |
### IsoLoadOptions() {#IsoLoadOptions--}
```
public IsoLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Mendapatkan sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak.

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive(\"archive.iso\", loadOptions);
 
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

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive(\"archive.iso\", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

