---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "アーカイブ内の単一ファイルを表します。"
type: docs
weight: 98
url: /ja/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

アーカイブ内の単一ファイルを表します。

[RarArchiveEntry](../../com.aspose.zip/rararchiveentry) インスタンスを [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) にキャストして、エントリが暗号化されているかどうかを判断します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getCompressedSize()](#getCompressedSize--) | 圧縮ファイルのサイズを取得します。 |
| [getCreationTime()](#getCreationTime--) | 作成日時を取得します。 |
| [getExtractionProgressed()](#getExtractionProgressed--) | 生ストリームの一部が抽出されたときに発生するイベントを取得します。 |
| [getLastAccessTime()](#getLastAccessTime--) | 最終アクセス日時を取得します。 |
| [getLength()](#getLength--) | 長さを取得します。 |
| [getModificationTime()](#getModificationTime--) | 最終更新日時を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | 元ファイルのサイズを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [open()](#open--) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |
| [open(String password)](#open-java.lang.String-) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 生ストリームの一部が抽出されたときに発生するイベントを設定します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。


パスワードを使用して RAR アーカイブのエントリを抽出します。

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 出力先ストリーム。書き込み可能である必要があります。 |
| パスワード | java.lang.String | 復号用のオプションパスワード。 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


エントリを提供されたパスでファイルシステムに抽出します。


RAR アーカイブから 2 つのエントリを抽出します。

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
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


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルがすでに存在する場合は上書きされます。 |
| パスワード | java.lang.String | 復号用のオプションパスワード。 |

**Returns:**
java.io.File - 抽出されたファイルの情報
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


圧縮ファイルのサイズを取得します。

**Returns:**
long - 圧縮ファイルのサイズ
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


作成日時を取得します。

**Returns:**
java.util.Date - 作成日時
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


生ストリームの一部が抽出されたときに発生するイベントを取得します。

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
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
long - the size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

ストリームから読み取り、ファイルの元の内容を取得します。例のセクションをご覧ください。

**Returns:**
java.io.InputStream - エントリの内容を表すストリーム
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。


使用方法:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

イベント送信者は [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) インスタンスです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 生のストリームの一部が抽出されたときに発生するイベントです。 |

