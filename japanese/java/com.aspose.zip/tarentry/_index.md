---
title: "TarEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "tar アーカイブ内の単一ファイルを表します。"
type: docs
weight: 126
url: /ja/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

tar アーカイブ内の単一ファイルを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getModificationTime()](#getModificationTime--) | ファイルまたはディレクトリの更新時刻を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | 元のファイルのサイズを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [open()](#open--) | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| [setName(String value)](#setName-java.lang.String-) | アーカイブ内のエントリの名前を設定します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

tar アーカイブのエントリを抽出します。

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |

**Returns:**
java.io.File - 抽出されたファイルの情報
### getLength() {#getLength--}
```
public final Long getLength()
```


エントリの長さ（バイト単位）を取得します。

**Returns:**
java.lang.Long - エントリのバイト単位の長さ
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


ファイルまたはディレクトリの更新時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリの最終更新時刻。
### getName() {#getName--}
```
public final String getName()
```


アーカイブ内のエントリ名を取得します。

**Returns:**
java.lang.String - アーカイブ内のエントリの名前
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


元のファイルのサイズを取得します。

`Length`([getLength](../../com.aspose.zip/tarentry\\#getLength--)) と同じ値です。

**Returns:**
long - 元のファイルのサイズ。
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


エントリがディレクトリを表すかどうかを示す値を取得します。

**Returns:**
boolean - エントリがディレクトリを表すかどうかを示す値
### open() {#open--}
```
public final InputStream open()
```


エントリを抽出用に開き、エントリの内容を含むストリームを提供します。


使用方法:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

