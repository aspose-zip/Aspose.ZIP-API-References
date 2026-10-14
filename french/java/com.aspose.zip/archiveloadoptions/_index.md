---
title: "ArchiveLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options avec lesquelles l'archive ZIP est chargée à partir d'un fichier compressé."
type: docs
weight: 35
url: /fr/java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

Options avec lesquelles l'archive ZIP est chargée à partir d'un fichier compressé.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Obtient le mot de passe pour déchiffrer les entrées. |
| [getEncoding()](#getEncoding--) | Obtient l'encodage des noms des entrées. |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Obtient un événement qui est déclenché lorsque des octets ont été extraits. |
| [getEntryListed()](#getEntryListed--) | Obtient un événement qui est déclenché lorsqu'une entrée est répertoriée dans la table des matières. |
| [getForwardOnly()](#getForwardOnly--) | Obtient le drapeau indiquant que l'archive est extraite d'un flux en lecture seule. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Obtient une valeur indiquant si la vérification du contrôle de somme des entrées ZIP doit être sautée et les discordances ignorées. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Définit le mot de passe pour déchiffrer les entrées. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit l'encodage des noms des entrées. |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Définit un événement qui est déclenché lorsque des octets ont été extraits. |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Définit un événement qui est déclenché lorsqu'une entrée est répertoriée dans la table des matières. |
| [setForwardOnly(boolean value)](#setForwardOnly-boolean-) | Définit le drapeau indiquant que l'archive est extraite d'un flux en lecture seule. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Définit une valeur indiquant si la vérification du contrôle de somme des entrées ZIP doit être sautée et les discordances ignorées. |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Obtient le mot de passe pour déchiffrer les entrées.


Vous pouvez fournir le mot de passe de déchiffrement une fois lors de l'extraction de l'archive.

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
java.nio.charset.Charset - l'encodage des noms d'entrées
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


Obtient un événement qui est déclenché lorsque des octets ont été extraits.

Suivre la progression de l'extraction d'une entrée.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
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

L'expéditeur d'événement est l'instance [ArchiveEntry](../../com.aspose.zip/archiveentry) dont l'extraction progresse.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


Obtient un événement qui est déclenché lorsqu'une entrée est répertoriée dans la table des matières.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
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

L'annulation entraîne généralement que certaines données ne sont pas extraites.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | un indicateur d'annulation utilisé pour annuler l'opération d'extraction. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Définit le mot de passe pour déchiffrer les entrées.


Vous pouvez fournir le mot de passe de déchiffrement une fois lors de l'extraction de l'archive.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.nio.charset.Charset | l'encodage des noms d'entrées |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Définit un événement qui est déclenché lorsque des octets ont été extraits.

Suivre la progression de l'extraction d'une entrée.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
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

L'expéditeur d'événement est l'instance [ArchiveEntry](../../com.aspose.zip/archiveentry) dont l'extraction progresse.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | un événement qui est déclenché lorsque certains octets ont été extraits |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


Définit un événement qui est déclenché lorsqu'une entrée est répertoriée dans la table des matières.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
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

