---
title: "CpioEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "cpio アーカイブ内の単一ファイルを表します。"
type: docs
weight: 58
url: /ja/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

cpio アーカイブ内の単一ファイルを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | 最後の書き込み時刻を取得します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getParent()](#getParent--) | エントリが属するアーカイブを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [open()](#open--) | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| [toString()](#toString--) | [CpioEntry](../../com.aspose.zip/cpioentry) クラスのインスタンスの文字列表現を返します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

cpio アーカイブからエントリを抽出します。

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |

**Returns:**
java.io.File - 抽出されたファイルの情報
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


最後の書き込み時刻を取得します。

**Returns:**
java.util.Date - 最後の書き込み時間
### getLength() {#getLength--}
```
public final Long getLength()
```


エントリの長さ（バイト単位）を取得します。

**Returns:**
java.lang.Long - エントリのバイト単位の長さ
### getName() {#getName--}
```
public final String getName()
```


アーカイブ内のエントリ名を取得します。

**Returns:**
java.lang.String - アーカイブ内のエントリの名前
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


エントリが属するアーカイブを取得します。

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


エントリがディレクトリを表すかどうかを示す値を取得します。

**Returns:**
boolean - エントリがディレクトリを表すかどうかを示す値。
### open() {#open--}
```
public final InputStream open()
```


エントリを抽出用に開き、エントリの内容を含むストリームを提供します。

使用方法:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
