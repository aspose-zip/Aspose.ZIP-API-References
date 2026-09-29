---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "圧縮ファイルからロードされる際のオプション。"
type: docs
weight: 116
url: /ja/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

圧縮ファイルから [SevenZipArchive](../../com.aspose.zip/sevenziparchive) をロードする際のオプション。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | エントリとエントリ名を復号化するためのパスワードを取得します。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | エントリとエントリ名を復号化するためのパスワードを設定します。 |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


エントリとエントリ名を復号化するためのパスワードを取得します。

アーカイブの抽出時に復号化パスワードを一度だけ提供できます。

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

