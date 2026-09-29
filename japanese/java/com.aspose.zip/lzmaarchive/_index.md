---
title: "LzmaArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは LZMA アーカイブファイルを表します。"
type: docs
weight: 86
url: /ja/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

このクラスは LZMA アーカイブ ファイルを表します。LZMA アーカイブの作成または抽出に使用します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | 新しいインスタンスの [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスを初期化し、lzma 形式でアーカイブを作成します。 |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | 新しいインスタンスの [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスを初期化し、lzma 形式でアーカイブを作成します。 |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | 解凍用に準備された [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスの新しいインスタンスを初期化します。 |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | 解凍用に準備された [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzma アーカイブをファイルに抽出します。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzma アーカイブをストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | パスで指定されたファイルに lzma アーカイブを抽出します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブの内容を指定されたディレクトリに抽出します。 |
| [getFileEntries()](#getFileEntries--) | lzma アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getLength()](#getLength--) | 長さを取得します。 |
| [getName()](#getName--) | 元のファイル名。 |
| [save(File destination)](#save-java.io.File-) | 指定された宛先ファイルに lzma アーカイブを保存します。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 指定されたストリームに lzma アーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 指定された宛先ファイルに lzma アーカイブを保存します。 |
| [setSource(File file)](#setSource-java.io.File-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


新しいインスタンスの [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスを初期化し、lzma 形式でアーカイブを作成します。

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


新しいインスタンスの [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスを初期化し、lzma 形式でアーカイブを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | 特定の lzma アーカイブの設定セット。 |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


解凍用に準備された [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスの新しいインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


解凍用に準備された [LzmaArchive](../../com.aspose.zip/lzmaarchive) クラスの新しいインスタンスを初期化します。

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル | java.io.File | 解凍されたデータを保存するファイル |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


lzma アーカイブをストリームに抽出します。

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 解凍されたデータを保存するファイルへのパス |

**Returns:**
java.io.File - 抽出されたファイルの情報
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


アーカイブの内容を指定されたディレクトリに抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 抽出されたファイルを配置するディレクトリへのパス |

ディレクトリが存在しない場合は作成されます |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


lzma アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - lzma アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリ。
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


アーカイブ形式を取得します。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


長さを取得します。

**Returns:**
java.lang.Long - 長さ
### getName() {#getName--}
```
public final String getName()
```


元のファイル名。

**Returns:**
java.lang.String - 元のファイル名
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


指定された宛先ファイルに lzma アーカイブを保存します。

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lzma"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
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


指定された宛先ファイルに lzma アーカイブを保存します。

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.lzma");
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

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
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

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.lzma");
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

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourcePath | java.lang.String | 入力ストリームとして開かれるファイルへのパス |

