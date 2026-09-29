---
title: "SevenZipLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры, с помощью которых  загружается из сжатого файла."
type: docs
weight: 116
url: /ru/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Параметры, с помощью которых [SevenZipArchive](../../com.aspose.zip/sevenziparchive) загружается из сжатого файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Получает пароль для расшифровки записей и имён записей. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Устанавливает пароль для расшифровки записей и имён записей. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Получает пароль для расшифровки записей и имён записей.

Вы можете указать пароль для расшифровки один раз при извлечении архива.

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

Отмена обычно приводит к тому, что некоторые данные не извлекаются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | Флаг отмены, используемый для прерывания операции извлечения. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Устанавливает пароль для расшифровки записей и имён записей.

Вы можете указать пароль для расшифровки один раз при извлечении архива.

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

