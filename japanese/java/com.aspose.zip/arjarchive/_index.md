---
title: "ArjArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは ARJ アーカイブ ファイルを表します。"
type: docs
weight: 37
url: /ja/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

このクラスは ARJ アーカイブ ファイルを表します。

次の圧縮方式のみがサポートされています:

| ------ | ------------------------------------------------------------ |
| メソッド | 説明 |
| 0      | 非圧縮 |
| 1      | LZ77 と適応ハフマン符号化の組み合わせ。最高の圧縮率。 |
| 2      | LZ77 と適応ハフマン符号化の組み合わせ。 |
| 3      | LZ77 と適応ハフマン符号化の組み合わせ。最高の速度。 |
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | 新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | 新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | 新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | 新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 指定されたディレクトリにすべてのエントリを抽出します。 |
| [getCommentary()](#getCommentary--) | コメントを取得します。 |
| [getEntries()](#getEntries--) | ARJ アーカイブを構成する [ArjEntryPlain](../../com.aspose.zip/arjentryplain) 型のエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) タイプのエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getName()](#getName--) | 元の名前を取得します。 |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

このコンストラクタはエントリを解凍しません。解凍するには [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | アーカイブのソース |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

このコンストラクタはエントリを解凍しません。解凍するには [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | アーカイブのソース |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


新しい [ArjArchive](../../com.aspose.zip/arjarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```

``````

try (ArjArchive archive = new ArjArchive(\"archive.arj\")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

このコンストラクタはエントリを展開しません。解凍するには [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


指定されたディレクトリにすべてのエントリを抽出します。

以下の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream(\"archive.arj\"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
