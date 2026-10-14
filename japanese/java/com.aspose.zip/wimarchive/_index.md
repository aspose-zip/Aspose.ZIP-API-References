---
title: "WimArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは wim アーカイブファイルを表します。"
type: docs
weight: 130
url: /ja/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

このクラスは wim アーカイブファイルを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | 新しい [WimArchive](../../com.aspose.zip/wimarchive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | 新しい [WimArchive](../../com.aspose.zip/wimarchive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | 新しい [WimArchive](../../com.aspose.zip/wimarchive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | 新しい [WimArchive](../../com.aspose.zip/wimarchive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | パスで指定されたファイルにアーカイブを抽出します。 |
| [getBootImageIndex()](#getBootImageIndex--) | 起動可能イメージの（0 ベース）インデックスを取得します。 |
| [getEntries()](#getEntries--) | アーカイブを構成する [WimEntry](../../com.aspose.zip/wimentry) 型のエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | wim アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFileFormatVersion()](#getFileFormatVersion--) | ファイル形式のバージョンを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getGuid()](#getGuid--) | アーカイブの識別 UUID を取得します。 |
| [getImages()](#getImages--) | アーカイブを構成する [WimImage](../../com.aspose.zip/wimimage) 型のエントリを取得します。 |
| [getManifest()](#getManifest--) | ファイルと含まれるイメージを記述する埋め込みマニフェストを取得します。 |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


新しい [WimArchive](../../com.aspose.zip/wimarchive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

以下の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream(\"archive.wim\"))) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

このコンストラクタはエントリを展開しません。展開については [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソース |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


新しい [WimArchive](../../com.aspose.zip/wimarchive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

以下の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

このコンストラクタはエントリを展開しません。展開については [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


パスで指定されたファイルにアーカイブを抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 抽出されたファイルを配置するディレクトリへのパス |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


起動可能イメージの（0 ベース）インデックスを取得します。

**Returns:**
int - 起動可能イメージの（ゼロベース）インデックス
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


アーカイブを構成する [WimEntry](../../com.aspose.zip/wimentry) 型のエントリを取得します。

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - アーカイブを構成するエントリ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


wim アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - wim アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリ
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


ファイル形式のバージョンを取得します。

**Returns:**
int - ファイル形式のバージョン
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


アーカイブ形式を取得します。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


アーカイブの識別 UUID を取得します。

**Returns:**
java.util.UUID - アーカイブを識別する UUID
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


アーカイブを構成する [WimImage](../../com.aspose.zip/wimimage) 型のエントリを取得します。

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - アーカイブを構成する [WimImage](../../com.aspose.zip/wimimage) 型のエントリ
### getManifest() {#getManifest--}
```
public final String getManifest()
```


ファイルと含まれるイメージを記述する埋め込みマニフェストを取得します。

**Returns:**
java.lang.String - ファイルと含まれるイメージを記述する埋め込みマニフェスト
