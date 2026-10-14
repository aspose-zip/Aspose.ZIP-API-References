---
title: "LzipArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは Lzip アーカイブファイルを表します。"
type: docs
weight: 83
url: /ja/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

このクラスは Lzip アーカイブ ファイルを表します。Lzip アーカイブの作成または抽出に使用します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | 新しい [LzipArchive](../../com.aspose.zip/lziparchive) のインスタンスを初期化します。 |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | 新しい [LzipArchive](../../com.aspose.zip/lziparchive) のインスタンスを初期化します。 |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | 解凍用に準備された [LzipArchive](../../com.aspose.zip/lziparchive) クラスの新しいインスタンスを初期化します。 |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | 解凍用に準備された [LzipArchive](../../com.aspose.zip/lziparchive) クラスの新しいインスタンスを初期化します。 |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | 解凍用に準備された [LzipArchive](../../com.aspose.zip/lziparchive) クラスの新しいインスタンスを初期化します。 |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | 解凍用に準備された [LzipArchive](../../com.aspose.zip/lziparchive) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzip アーカイブをファイルに抽出します。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzip アーカイブをストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | パスで指定されたファイルに lzip アーカイブを抽出します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブの内容を指定されたディレクトリに抽出します。 |
| [getFileEntries()](#getFileEntries--) | lzip アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getLength()](#getLength--) | 長さを取得します。 |
| [getName()](#getName--) | 元のファイル名。 |
| [getSettings()](#getSettings--) | 特定の lzip アーカイブの設定を取得します。 |
| [getUncompressedSize()](#getUncompressedSize--) | ファイルデータの非圧縮サイズ（バイト単位）を取得します。 |
| [save(File destination)](#save-java.io.File-) | 提供された宛先ファイルに lzip アーカイブを保存します。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 提供されたストリームに lzip アーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 提供された宛先ファイルに lzip アーカイブを保存します。 |
| [setSource(File file)](#setSource-java.io.File-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(String path)](#setSource-java.lang.String-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


新しい [LzipArchive](../../com.aspose.zip/lziparchive) のインスタンスを初期化します。

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


新しい [LzipArchive](../../com.aspose.zip/lziparchive) のインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | 辞書サイズの定義を含む特定の lzip アーカイブの設定 |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


解凍用に準備された [LzipArchive](../../com.aspose.zip/lziparchive) クラスの新しいインスタンスを初期化します。

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

このコンストラクタは解凍しません。解凍するには [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソース |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | アーカイブをロードするためのオプションです。 |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


解凍用に準備された [LzipArchive](../../com.aspose.zip/lziparchive) クラスの新しいインスタンスを初期化します。

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

このコンストラクタは解凍しません。解凍するには [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブのソースへのパス |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | アーカイブをロードするためのオプションです。 |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


lzip アーカイブをファイルに抽出します。

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
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


パスで指定されたファイルに lzip アーカイブを抽出します。

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
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


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.File | ファイルは、宛先ストリームとして開かれます |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


提供されたストリームに lzip アーカイブを保存します。

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブの入力ストリーム |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

