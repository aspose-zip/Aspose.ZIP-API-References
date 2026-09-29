---
title: "ArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen ein ZIP-Archiv aus einer komprimierten Datei geladen wird."
type: docs
weight: 35
url: /de/java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

Optionen, mit denen ein ZIP-Archiv aus einer komprimierten Datei geladen wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Gibt das Passwort zum Entschlüsseln von Einträgen zurück. |
| [getEncoding()](#getEncoding--) | Gibt die Kodierung für die Namen der Einträge zurück. |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn einige Bytes extrahiert wurden. |
| [getEntryListed()](#getEntryListed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Eintrag im Inhaltsverzeichnis aufgeführt wird. |
| [getForwardOnly()](#getForwardOnly--) | Gibt das Flag zurück, das anzeigt, dass das Archiv aus einem schreibgeschützten Stream extrahiert wurde. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Gibt einen Wert zurück, der angibt, ob die Prüfsummenprüfung der ZIP‑Einträge übersprungen und Diskrepanzen ignoriert werden sollen. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Setzt das Passwort zum Entschlüsseln von Einträgen. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Setzt die Kodierung für die Namen der Einträge. |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn einige Bytes extrahiert wurden. |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Eintrag im Inhaltsverzeichnis aufgeführt wird. |
| [setForwardOnly(boolean value)](#setForwardOnly-boolean-) | Setzt das Flag, das anzeigt, dass das Archiv aus einem schreibgeschützten Stream extrahiert wurde. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Setzt einen Wert, der angibt, ob die Prüfsummenprüfung der ZIP‑Einträge übersprungen und Diskrepanzen ignoriert werden sollen. |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Gibt das Passwort zum Entschlüsseln von Einträgen zurück.


Sie können das Entschlüsselungspasswort einmalig bei der Archivextraktion angeben.

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
java.nio.charset.Charset - die Kodierung für die Namen von Einträgen
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn einige Bytes extrahiert wurden.

Verfolgen Sie den Fortschritt einer Eintrags-Extraktion.

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

Event sender ist die [ArchiveEntry](../../com.aspose.zip/archiveentry) Instanz, deren Extraktion fortschreitet.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Eintrag im Inhaltsverzeichnis aufgeführt wird.

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

Ein Abbruch führt meistens dazu, dass einige Daten nicht extrahiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | Ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Setzt das Passwort zum Entschlüsseln von Einträgen.


Sie können das Entschlüsselungspasswort einmalig bei der Archivextraktion angeben.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.nio.charset.Charset | die Kodierung für die Namen von Einträgen |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, wenn einige Bytes extrahiert wurden.

Verfolgen Sie den Fortschritt einer Eintrags-Extraktion.

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

Event sender ist die [ArchiveEntry](../../com.aspose.zip/archiveentry) Instanz, deren Extraktion fortschreitet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn einige Bytes extrahiert wurden |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, wenn ein Eintrag im Inhaltsverzeichnis aufgeführt wird.

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

