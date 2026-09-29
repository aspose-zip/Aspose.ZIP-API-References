---
title: "IsoEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ISO アーカイブ内のエントリ ファイルまたはディレクトリを表します。"
type: docs
weight: 72
url: /ja/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

ISO アーカイブ内のエントリ (ファイルまたはディレクトリ) を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getLength()](#getLength--) | エントリの長さを取得します。 |
| [getModificationTime()](#getModificationTime--) | 最終更新日時を取得します。 |
| [getName()](#getName--) | エントリの名前を取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリかどうかを示す値を取得します。 |
| [toString()](#toString--) | 現在のエントリを表す文字列を返します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 宛先ストリーム |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


エントリを提供されたパスでファイルシステムに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |

**Returns:**
java.io.File - 抽出されたデータを含む java.io.File インスタンス
### getLength() {#getLength--}
```
public Long getLength()
```


エントリの長さを取得します。

**Returns:**
java.lang.Long - エントリの長さ
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


最終更新日時を取得します。

**Returns:**
java.util.Date - 最終更新日時
### getName() {#getName--}
```
public final String getName()
```


エントリの名前を取得します。

**Returns:**
java.lang.String - エントリの名前
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


エントリがディレクトリかどうかを示す値を取得します。

**Returns:**
boolean - エントリがディレクトリを表すかどうかを示す値
### toString() {#toString--}
```
public String toString()
```


現在のエントリを表す文字列を返します。

**Returns:**
java.lang.String - エントリの名前
