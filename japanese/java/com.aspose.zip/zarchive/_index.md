---
title: "ZArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは Z compress アーカイブファイルを表します。"
type: docs
weight: 153
url: /ja/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

このクラスは Z（compress）アーカイブファイルを表します。Z アーカイブの作成や抽出に使用します。

参照: [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ZArchive()](#ZArchive--) | 圧縮用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。 |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | 解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。 |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | 解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。 |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | 解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。 |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | 解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Z アーカイブをファイルに抽出します。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Z アーカイブをストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | パスで指定されたファイルに Z アーカイブを抽出します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブの内容を指定されたディレクトリに抽出します。 |
| [getFileEntries()](#getFileEntries--) | Z アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリの名前を取得します。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 提供されたストリームに Z アーカイブを保存します。 |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | 提供されたストリームに Z アーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 提供された宛先ファイルに Z アーカイブを保存します。 |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | 提供された宛先ファイルに Z アーカイブを保存します。 |
| [setSource(File file)](#setSource-java.io.File-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


圧縮用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | アーカイブを読み込むためのオプション |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブのソースへのパス |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


解凍用に準備された [ZArchive](../../com.aspose.zip/zarchive) クラスの新しいインスタンスを初期化します。

このコンストラクタは解凍しません。解凍するには [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブのソースへのパス |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | アーカイブを読み込むためのオプション |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Z アーカイブをファイルに抽出します。

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


パスで指定されたファイルに Z アーカイブを抽出します。

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | java.io.OutputStream | 宛先ストリーム |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


提供されたストリームに Z アーカイブを保存します。

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


提供された宛先ファイルに Z アーカイブを保存します。

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル | java.io.File | 入力ストリームとして開かれるファイル情報 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourcePath | java.lang.String | 入力ストリームとして開かれるファイルへのパス |

