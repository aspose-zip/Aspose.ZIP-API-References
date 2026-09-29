---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "アーカイブ インスタンスに関する情報を表します。"
type: docs
weight: 34
url: /ja/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

アーカイブ インスタンスに関する情報を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | アーカイブ内のエントリ（ファイル）の名前が暗号化されているかどうかを示す値を取得します。 |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | アーカイブ形式情報を取得します。 |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | アーカイブ形式情報を取得します。 |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | アーカイブインスタンス情報を取得します。 |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | アーカイブインスタンス情報を取得します。 |
| [getFormatInfo()](#getFormatInfo--) | アーカイブ形式情報を取得します。 |
| [isContentEncrypted()](#isContentEncrypted--) | アーカイブの内容が暗号化されているかどうかを示す値を取得します。 |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


アーカイブ内のエントリ（ファイル）の名前が暗号化されているかどうかを示す値を取得します。

**Returns:**
boolean - アーカイブ内のエントリ（ファイル）の名前が暗号化されているかどうかを示す値。
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


アーカイブ形式情報を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | アーカイブファイルのストリームです。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


アーカイブ形式情報を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | アーカイブファイルのファイル名です。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


アーカイブインスタンス情報を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | アーカイブファイルのストリームです。 |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


アーカイブインスタンス情報を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | アーカイブファイルのファイル名です。 |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


アーカイブ形式情報を取得します。

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


アーカイブの内容が暗号化されているかどうかを示す値を取得します。

**Returns:**
boolean - アーカイブの内容が暗号化されているかどうかを示す値。
