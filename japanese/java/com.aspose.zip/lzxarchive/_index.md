---
title: "LzxArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは LZX .lzx アーカイブファイルを表します。"
type: docs
weight: 89
url: /ja/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

このクラスは LZX (.lzx) アーカイブファイルを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | 新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | 新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | 新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | 新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブ内のすべてのファイルとディレクトリを指定されたディレクトリへ抽出します。 |
| [getEntries()](#getEntries--) | アーカイブを構成する [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) タイプのファイルエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) タイプのエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

このコンストラクタはエントリを展開しません。展開するには [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | アーカイブのソースです。 |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

このコンストラクタはエントリを展開しません。展開するには [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | アーカイブのソースです。 |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


新しい [LzxArchive](../../com.aspose.zip/lzxarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

次の例ではアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

このコンストラクタはエントリを展開しません。展開するには [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


アーカイブ内のすべてのファイルとディレクトリを指定されたディレクトリへ抽出します。

```

``````

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
