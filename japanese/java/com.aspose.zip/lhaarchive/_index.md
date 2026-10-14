---
title: "LhaArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは LHA .lzh アーカイブファイルを表します。"
type: docs
weight: 75
url: /ja/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

このクラスは LHA (.lzh) アーカイブファイルを表します。

次の圧縮方式のみがサポートされています:

| ------ | --------------------------------------------- |
| メソッド | 説明                                   |
| lh0    | 非圧縮                                  |
| lh4    | 8 KiB スライディング辞書と静的ハフマン   |
| lh5    | 16 KiB スライディング辞書と静的ハフマン  |
| lh6    | 64 KiB スライディング辞書と静的ハフマン  |
| lh7    | 128 KiB のスライディング辞書とスタティックハフマン |
| lhx    | 1 Mib のスライディング辞書とスタティックハフマン   |
| lhd    | ディレクトリ                                     |
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | 新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | 新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | 新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | 新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブ内のすべてのファイルとディレクトリを指定されたディレクトリへ抽出します。 |
| [getEntries()](#getEntries--) | アーカイブを構成する [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) 型のファイルエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) タイプのエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

このコンストラクタはエントリを展開しません。展開するには [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソース |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

このコンストラクタはエントリを展開しません。展開するには [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソース |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


新しい [LhaArchive](../../com.aspose.zip/lhaarchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

次の例ではアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive(\"sample.lzh\")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

このコンストラクタはエントリを展開しません。展開するには [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブ ファイルへの完全修飾パスまたは相対パス |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

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

try (LhaArchive archive = new LhaArchive(\"archive.lzh\")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
