---
title: "XzArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは xz アーカイブ ファイルを表します。"
type: docs
weight: 146
url: /ja/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

このクラスは xz アーカイブ ファイルを表します。xz アーカイブの作成と抽出に使用します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [XzArchive()](#XzArchive--) | 新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化し、xz 形式でアーカイブを作成します。 |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | 新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化し、xz 形式でアーカイブを作成します。 |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | 解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。 |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | 解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。 |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | 解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。 |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | 解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | xz アーカイブをファイルに抽出します。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | xz アーカイブをストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | パスで指定されたファイルに xz アーカイブを抽出します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブの内容を指定されたディレクトリに抽出します。 |
| [getFileEntries()](#getFileEntries--) | xz アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリの名前を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | ファイルデータの非圧縮サイズ（バイト単位）を取得します。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 提供されたストリームに xz アーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 提供された宛先ファイルに xz アーカイブを保存します。 |
| [setSource(File file)](#setSource-java.io.File-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化し、xz 形式でアーカイブを作成します。

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化し、xz 形式でアーカイブを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | アーカイブをロードするためのオプションです。 |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブのソースへのパス |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


解凍用に準備された新しい [XzArchive](../../com.aspose.zip/xzarchive) クラスのインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブのソースへのパス |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


xz アーカイブをファイルに抽出します。

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 解凍データを格納するストリーム |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


パスで指定されたファイルに xz アーカイブを抽出します。

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | java.io.OutputStream | 宛先ストリーム |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


提供された宛先ファイルに xz アーカイブを保存します。

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File("data.bin"));
archive.save(\"result.xz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル | java.io.File | 入力ストリームとして開かれるファイル |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourcePath | java.lang.String | 入力ストリームとして開かれるファイルへのパス |

