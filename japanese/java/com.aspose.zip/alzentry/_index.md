---
title: "AlzEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ALZ アーカイブ内のファイル エントリとそのメタデータを表します。"
type: docs
weight: 13
url: /ja/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

ALZ アーカイブ内のファイル エントリとそのメタデータを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを書き込み可能なストリームに抽出します。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | エントリをオプションのパスワードを使用して書き込み可能なストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを指定されたファイルに抽出します。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | エントリをオプションのパスワードを使用して指定されたファイルに抽出します。 |
| [getCompressedSize()](#getCompressedSize--) | エントリデータの圧縮サイズ（バイト単位）を取得します。 |
| [getLength()](#getLength--) | このエントリの非圧縮長さを取得します。 |
| [getName()](#getName--) | アーカイブに保存されているエントリ名を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | エントリデータの非圧縮サイズ（バイト単位）を取得します。 |
| [isDirectory()](#isDirectory--) | このエントリがディレクトリかどうかを取得します。 |
| [open()](#open--) | エントリを開き、展開されたデータを含むストリームを提供します。 |
| [open(String password)](#open-java.lang.String-) | エントリを開き、展開されたデータを含むストリームを提供します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを書き込み可能なストリームに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 宛先ストリーム |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


エントリをオプションのパスワードを使用して書き込み可能なストリームに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 宛先ストリーム |
| パスワード | java.lang.String | このエントリのオプションのパスワード |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


エントリを指定されたファイルに抽出します。既存のファイルは上書きされます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルパス |

**Returns:**
java.io.File - 抽出されたファイル
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


エントリをオプションのパスワードを使用して指定されたファイルに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルパス |
| パスワード | java.lang.String | このエントリのオプションのパスワード |

**Returns:**
java.io.File - 抽出されたファイル
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


エントリデータの圧縮サイズ（バイト単位）を取得します。

**Returns:**
long - 圧縮サイズ（バイト）
### getLength() {#getLength--}
```
public final Long getLength()
```


このエントリの非圧縮長さを取得します。

**Returns:**
java.lang.Long - 非圧縮長さ（バイト）
### getName() {#getName--}
```
public final String getName()
```


アーカイブに保存されているエントリ名を取得します。

**Returns:**
java.lang.String - エントリ名
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


エントリデータの非圧縮サイズ（バイト単位）を取得します。

**Returns:**
long - 非圧縮サイズ（バイト）
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


このエントリがディレクトリかどうかを取得します。

**Returns:**
boolean - ディレクトリエントリの場合は `true`
### open() {#open--}
```
public final InputStream open()
```


エントリを開き、展開されたデータを含むストリームを提供します。

**Returns:**
java.io.InputStream - 展開されたエントリデータを含むストリーム
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


エントリを開き、展開されたデータを含むストリームを提供します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パスワード | java.lang.String | このエントリのオプションのパスワード |

**Returns:**
java.io.InputStream - 展開されたエントリデータを含むストリーム
