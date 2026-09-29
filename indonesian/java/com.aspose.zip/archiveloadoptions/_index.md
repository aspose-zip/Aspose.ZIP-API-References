---
title: "ArchiveLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi yang digunakan untuk memuat arsip ZIP dari file terkompresi."
type: docs
weight: 35
url: /id/java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

Opsi yang digunakan untuk memuat arsip ZIP dari file terkompresi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Mendapatkan kata sandi untuk mendekripsi entri. |
| [getEncoding()](#getEncoding--) | Mendapatkan pengkodean untuk nama entri. |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Mendapatkan sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak. |
| [getEntryListed()](#getEntryListed--) | Mendapatkan sebuah peristiwa yang dipicu ketika sebuah entri terdaftar dalam daftar isi. |
| [getForwardOnly()](#getForwardOnly--) | Mendapatkan flag yang menunjukkan bahwa arsip diekstrak dari aliran hanya-baca. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Mendapatkan nilai yang menunjukkan apakah verifikasi checksum dari entri ZIP dilewati dan ketidaksesuaian diabaikan. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Mengatur kata sandi untuk mendekripsi entri. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur pengkodean untuk nama entri. |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Mengatur sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak. |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Mengatur sebuah peristiwa yang dipicu ketika sebuah entri terdaftar dalam daftar isi. |
| [setForwardOnly(boolean value)](#setForwardOnly-boolean-) | Mengatur flag yang menunjukkan bahwa arsip diekstrak dari aliran hanya-baca. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Mengatur nilai yang menunjukkan apakah verifikasi checksum dari entri ZIP dilewati dan ketidaksesuaian diabaikan. |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Mendapatkan kata sandi untuk mendekripsi entri.


Anda dapat menyediakan kata sandi dekripsi sekali saat ekstraksi arsip.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.zip")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets the encoding for entries' names.


Entry name composed using specified encoding regardless of zip file properties.

```

``````

    try (FileInputStream fs = new FileInputStream("archive.zip")) {
        ArchiveLoadOptions options = new ArchiveLoadOptions();
        options.setEncoding(Charset.forName("MS932"));
        try (Archive archive = new Archive(fs, options)) {
            String name = archive.getEntries().get(0).getName();
        }
    } catch (IOException ex) {
    }
 
```



**Returns:**
java.nio.charset.Charset - pengkodean untuk nama entri
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


Mendapatkan sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak.

Lacak kemajuan ekstraksi entri.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive("archive.zip", options);
 
```

Cancel an entry extraction after a certain time.

```

``````

     long startTime = System.nanoTime();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setEntryExtractionProgressed((s, e) -> {
         if ((System.nanoTime() - startTime) / 1_000_000 > 1000)
             e.setCancel(true);
     });
     try (Archive a = new Archive("big.zip", options)) {
         a.getEntries().get(0).extract("first.bin");
     }
 
```

Pengirim Event adalah instance [ArchiveEntry](../../com.aspose.zip/archiveentry) yang ekstraksinya sedang diproses.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


Mendapatkan sebuah peristiwa yang dipicu ketika sebuah entri terdaftar dalam daftar isi.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive("archive.zip", options);
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when an entry listed within table of content
### getForwardOnly() {#getForwardOnly--}
```
public final boolean getForwardOnly()
```


Gets the flag that indicating that archive is extracted from read-only stream.

**Returns:**
boolean - true, if archive's stream is rean-only, false elsewhere.
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public final boolean getSkipChecksumVerification()
```


Gets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Returns:**
boolean - a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ZIP archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (Archive a = new Archive("big.zip", options)) {
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

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Mengatur kata sandi untuk mendekripsi entri.


Anda dapat menyediakan kata sandi dekripsi sekali saat ekstraksi arsip.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.zip")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets the encoding for entries' names.


Entry name composed using specified encoding regardless of zip file properties.

```

``````

    try (FileInputStream fs = new FileInputStream("archive.zip")) {
        ArchiveLoadOptions options = new ArchiveLoadOptions();
        options.setEncoding(Charset.forName("MS932"));
        try (Archive archive = new Archive(fs, options)) {
            String name = archive.getEntries().get(0).getName();
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.nio.charset.Charset | pengkodean untuk nama entri |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Mengatur sebuah peristiwa yang dipicu ketika beberapa byte telah diekstrak.

Lacak kemajuan ekstraksi entri.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive("archive.zip", options);
 
```

Cancel an entry extraction after a certain time.

```

``````

     long startTime = System.nanoTime();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setEntryExtractionProgressed((s, e) -> {
         if ((System.nanoTime() - startTime) / 1_000_000 > 1000)
             e.setCancel(true);
     });
     try (Archive a = new Archive("big.zip", options)) {
         a.getEntries().get(0).extract("first.bin");
     }
 
```

Pengirim Event adalah instance [ArchiveEntry](../../com.aspose.zip/archiveentry) yang ekstraksinya sedang diproses.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | sebuah event yang dipicu ketika beberapa byte telah diekstrak |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


Mengatur sebuah peristiwa yang dipicu ketika sebuah entri terdaftar dalam daftar isi.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive("archive.zip", options);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | an event that is raised when an entry listed within table of content |

### setForwardOnly(boolean value) {#setForwardOnly-boolean-}
```
public final void setForwardOnly(boolean value)
```


Sets the flag that indicating that archive is extracted from read-only stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true, if archive's stream is rean-only, false elsewhere. |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public final void setSkipChecksumVerification(boolean value)
```


Sets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored |

