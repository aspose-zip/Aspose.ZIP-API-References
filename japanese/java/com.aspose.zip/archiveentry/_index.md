---
title: "ArchiveEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "アーカイブ内の単一ファイルを表します。"
type: docs
weight: 27
url: /ja/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

アーカイブ内の単一ファイルを表します。

[ArchiveEntry](../../com.aspose.zip/archiveentry) インスタンスを [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) にキャストして、エントリが暗号化されているかどうかを判断します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getComment()](#getComment--) | アーカイブ内のエントリのコメントを取得します。 |
| [getCompressedSize()](#getCompressedSize--) | 圧縮ファイルのサイズを取得します。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 生ストリームの一部が圧縮されたときに発生するイベントを取得します。 |
| [getCompressionSettings()](#getCompressionSettings--) | 圧縮または解凍の設定を取得します。 |
| [getDataSource()](#getDataSource--) | エントリがアーカイブに追加された場合のソースで、抽出されたものではありません。 |
| [getExtractionProgressed()](#getExtractionProgressed--) | 生ストリームの一部が抽出されたときに発生するイベントを取得します。 |
| [getLength()](#getLength--) | 長さを取得します。 |
| [getModificationTime()](#getModificationTime--) | 最終更新日時を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | 元ファイルのサイズを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [open()](#open--) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |
| [open(String password)](#open-java.lang.String-) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 生ストリームの一部が圧縮されたときに発生するイベントを設定します。 |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | 生ストリームの一部が抽出されたときに発生するイベントを設定します。 |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | 最終更新日時を設定します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

パスワードで zip アーカイブのエントリを抽出します。

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
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

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
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

ZIP アーカイブの 2 つのエントリをそれぞれ別々のパスワードで抽出します。

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
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
### getComment() {#getComment--}
```
public final String getComment()
```


アーカイブ内のエントリのコメントを取得します。

**Returns:**
java.lang.String - アーカイブ内エントリのコメント
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

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

このサンプルでは、エントリが最初の 100 MB 抽出された後にキャンセルするためにイベントハンドラが使用されています。

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
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


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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

ストリームから読み取り、ファイルの元の内容を取得します。

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
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
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

Event の送信者は [ArchiveEntry](../../com.aspose.zip/archiveentry) インスタンスです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 生ストリームの一部が圧縮されたときに発生するイベント |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


生ストリームの一部が抽出されたときに発生するイベントを設定します。

このサンプルでは、イベントハンドラは処理されたサイズの割合をパーセンテージで計算するために使用されます。

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender は [ArchiveEntry](../../com.aspose.zip/archiveentry) インスタンスです。抽出をキャンセルすることが可能です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | 生のストリームの一部が抽出されたときに発生するイベントです。 |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


最終更新日時を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 最終更新日時 |

