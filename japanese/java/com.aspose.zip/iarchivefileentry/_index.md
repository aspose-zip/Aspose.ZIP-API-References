---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このインターフェイスはアーカイブ ファイル エントリを表します。"
type: docs
weight: 162
url: /ja/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

このインターフェイスはアーカイブ ファイル エントリを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getName()](#getName--) | エントリの名前を取得します。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 宛先ストリーム。書き込み可能である必要があります。 |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
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
public abstract Long getLength()
```


エントリの長さ（バイト単位）を取得します。

**Returns:**
java.lang.Long - エントリのバイト単位の長さ
### getName() {#getName--}
```
public abstract String getName()
```


エントリの名前を取得します。

圧縮専用のアーカイブ（gzip、bzip2、lzip、lzma、xz、z など）は、ヘッダーで別の名前が見つからない限り、名前が "File.bin" になります。

**Returns:**
java.lang.String - エントリの名前
