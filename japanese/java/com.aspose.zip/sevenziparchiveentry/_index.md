---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7z アーカイブ内の単一ファイルを表します。"
type: docs
weight: 105
url: /ja/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

7z アーカイブ内の単一ファイルを表します。

[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) インスタンスを [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) にキャストして、エントリが暗号化されているかどうかを判断します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getCompressedSize()](#getCompressedSize--) | 圧縮ファイルのサイズを取得します。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 生ストリームの一部が圧縮されたときに発生するイベントを取得します。 |
| [getCompressionSettings()](#getCompressionSettings--) | 圧縮または解凍の設定を取得します。 |
| [getLength()](#getLength--) | 長さを取得します。 |
| [getModificationTime()](#getModificationTime--) | 最終更新日時を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | 元ファイルのサイズを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [open()](#open--) | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| [open(String password)](#open-java.lang.String-) | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 生ストリームの一部が圧縮されたときに発生するイベントを設定します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

パスワードで zip アーカイブのエントリを抽出します。

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 宛先ストリーム。書き込み可能である必要があります。 |
| パスワード | java.lang.String | 復号用のオプションパスワード |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


エントリを提供されたパスでファイルシステムに抽出します。

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract("data.bin");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |
| パスワード | java.lang.String | 復号用のオプションパスワード |

**Returns:**
java.io.File - 抽出されたファイルの情報
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


圧縮ファイルのサイズを取得します。

**Returns:**
long - 圧縮ファイルのサイズ
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


生ストリームの一部が圧縮されたときに発生するイベントを取得します。

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

ストリームから読み取り、ファイルの元の内容を取得します。例のセクションをご覧ください。

**Returns:**
java.io.InputStream - エントリの内容を表すストリーム
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


エントリを抽出用に開き、エントリの内容を含むストリームを提供します。

使用方法:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

イベント送信者は [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) インスタンスです。

LZMA2 エントリに対して、ソリッドモードおよびマルチスレッドモードでは呼び出されません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 生ストリームの一部が圧縮されたときに発生するイベント |

