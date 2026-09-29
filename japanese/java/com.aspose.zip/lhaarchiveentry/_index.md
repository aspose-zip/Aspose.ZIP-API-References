---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "Lha アーカイブ内の単一ファイルを表します。"
type: docs
weight: 76
url: /ja/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Lha アーカイブ内の単一ファイルを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Lha アーカイブエントリをファイルに抽出します。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | Lha アーカイブエントリをパスで指定されたファイルシステムに抽出します。 |
| [getLastModified()](#getLastModified--) | エントリの最終更新時刻を取得します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getModificationTime()](#getModificationTime--) | エントリの最終更新時刻を取得します。 |
| [getName()](#getName--) | エントリの名前を取得します。 |
| [getPath()](#getPath--) | エントリへのフルパスを取得します。 |
| [isDirectory()](#isDirectory--) | このエントリがディレクトリかどうかを示す値を取得します。 |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Lha アーカイブエントリをファイルに抽出します。

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 解凍されたデータを保存するファイルへのパス |

**Returns:**
java.io.File - 抽出されたデータを含む java.io.File インスタンス
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


エントリの最終更新時刻を取得します。

**Returns:**
java.util.Date - エントリの最終更新時刻
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


エントリの最終更新時刻を取得します。

**Returns:**
java.util.Date - エントリの最終更新時刻
### getName() {#getName--}
```
public final String getName()
```


エントリの名前を取得します。

圧縮専用のアーカイブ（gzip、bzip2、lzip、lzma、xz、z など）は、ヘッダーで別の名前が見つからない限り、名前が "File.bin" になります。

**Returns:**
java.lang.String - エントリの名前
### getPath() {#getPath--}
```
public final String getPath()
```


エントリへのフルパスを取得します。

**Returns:**
java.lang.String - エントリへのフルパス
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


このエントリがディレクトリかどうかを示す値を取得します。

**Returns:**
boolean - このエントリがディレクトリかどうかを示す値です。
