---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Sıkıştırılmış bir dosyadan  yüklenirken kullanılan seçenekler."
type: docs
weight: 116
url: /tr/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Sıkıştırılmış bir dosyadan [SevenZipArchive](../../com.aspose.zip/sevenziparchive) yüklenirken kullanılan seçenekler.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Girişleri ve giriş adlarını çözmek için şifreyi alır. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Girişleri ve giriş adlarını çözmek için şifreyi ayarlar. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Girişleri ve giriş adlarını çözmek için şifreyi alır.

Arşiv çıkarma sırasında bir kez şifre çözme şifresi sağlayabilirsiniz.

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

Cancellation çoğunlukla bazı verilerin çıkarılmamasına neden olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | çıkarma işlemini iptal etmek için kullanılan bir cancellation flag. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Girişleri ve giriş adlarını çözmek için şifreyi ayarlar.

Arşiv çıkarma sırasında bir kez şifre çözme şifresi sağlayabilirsiniz.

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

