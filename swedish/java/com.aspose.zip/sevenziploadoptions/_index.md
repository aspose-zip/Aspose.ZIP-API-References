---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ med vilka  laddas från en komprimerad fil."
type: docs
weight: 116
url: /sv/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Alternativ med vilka [SevenZipArchive](../../com.aspose.zip/sevenziparchive) laddas från en komprimerad fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Hämtar lösenordet för att dekryptera poster och postnamn. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Ställer in lösenordet för att dekryptera poster och postnamn. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Hämtar lösenordet för att dekryptera poster och postnamn.

Du kan ange avkrypteringslösenordet en gång vid arkivextraktion.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel 7Z archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setCancellationFlag(cf);
         try (SevenZipArchive a = new SevenZipArchive("big.7z", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

Avbrytning resulterar oftast i att vissa data inte extraheras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | en avbrytande flagga som används för att avbryta extraktionsoperationen. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Ställer in lösenordet för att dekryptera poster och postnamn.

Du kan ange avkrypteringslösenordet en gång vid arkivextraktion.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

