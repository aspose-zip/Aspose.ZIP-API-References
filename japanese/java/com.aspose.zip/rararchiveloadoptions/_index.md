---
title: "RarArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "圧縮ファイルからロードされる際のオプション。"
type: docs
weight: 101
url: /ja/java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

圧縮ファイルから [RarArchive](../../com.aspose.zip/rararchive) をロードする際のオプションです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | エントリとエントリ名を復号化するためのパスワードを取得します。 |
| [getDictionaryStorageMode()](#getDictionaryStorageMode--) | RAR 解凍辞書の格納方法を取得します。 |
| [getTemporaryDirectory()](#getTemporaryDirectory--) | 一時的な辞書ファイルに使用されるディレクトリを取得します。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | エントリとエントリ名を復号化するためのパスワードを設定します。 |
| [setDictionaryStorageMode(RarDictionaryStorageMode value)](#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-) | RAR 解凍辞書の格納方法を設定します。 |
| [setTemporaryDirectory(String value)](#setTemporaryDirectory-java.lang.String-) | 一時的な辞書ファイルに使用されるディレクトリを設定します。 |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


エントリとエントリ名を復号化するためのパスワードを取得します。

アーカイブの抽出時に復号化パスワードを一度だけ提供できます。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### getDictionaryStorageMode() {#getDictionaryStorageMode--}
```
public final RarDictionaryStorageMode getDictionaryStorageMode()
```


Gets how the RAR decompression dictionary is stored.

**Returns:**
[RarDictionaryStorageMode](../../com.aspose.zip/rardictionarystoragemode) - the dictionary storage mode
### getTemporaryDirectory() {#getTemporaryDirectory--}
```
public final String getTemporaryDirectory()
```


Gets the directory used for temporary dictionary files.

**Returns:**
java.lang.String - the temporary directory; the system temporary directory is used by default
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel RAR archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (RarArchive a = new RarArchive("big.rar", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

キャンセルは主に一部のデータが抽出されない結果となります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 抽出操作をキャンセルするために使用されるキャンセルフラグです。 |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


エントリとエントリ名を復号化するためのパスワードを設定します。

アーカイブの抽出時に復号化パスワードを一度だけ提供できます。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

### setDictionaryStorageMode(RarDictionaryStorageMode value) {#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-}
```
public final void setDictionaryStorageMode(RarDictionaryStorageMode value)
```


Sets how the RAR decompression dictionary is stored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RarDictionaryStorageMode](../../com.aspose.zip/rardictionarystoragemode) | the dictionary storage mode |

### setTemporaryDirectory(String value) {#setTemporaryDirectory-java.lang.String-}
```
public final void setTemporaryDirectory(String value)
```


Sets the directory used for temporary dictionary files. A null or empty value selects the system temporary directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the temporary directory |

