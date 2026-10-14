---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ARJ アーカイブ内の単一ファイルを表します。"
type: docs
weight: 38
url: /ja/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

ARJ アーカイブ内の単一ファイルを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | ARJ アーカイブ エントリをファイルに抽出します。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getCompressedSize()](#getCompressedSize--) | 圧縮ファイルのサイズを取得します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | 元ファイルのサイズを取得します。 |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


ARJ アーカイブ エントリをファイルに抽出します。

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |

**Returns:**
java.io.File - 組み立てられたファイルの情報
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


圧縮ファイルのサイズを取得します。

**Returns:**
long - 圧縮ファイルのサイズ
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
java.lang.String - アーカイブ内エントリの名前
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


元ファイルのサイズを取得します。

**Returns:**
long - 元のファイルのサイズ
