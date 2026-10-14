---
title: "GzipArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは gzip アーカイブファイルを表します。"
type: docs
weight: 69
url: /ja/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

このクラスは gzip アーカイブファイルを表します。gzip アーカイブの作成または抽出に使用します。

Gzip 圧縮アルゴリズムは DEFLATE アルゴリズムに基づいており、LZ77 とハフマン符号化の組み合わせです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | 圧縮用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | 解凍用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | 解凍用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | 解凍用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | 解凍用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | 新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | 新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 提供されたストリームへアーカイブを抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | パスで指定されたファイルにアーカイブを抽出します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブの内容を指定されたディレクトリに抽出します。 |
| [getFileEntries()](#getFileEntries--) | gzip アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getLength()](#getLength--) | 元のファイルのサイズを取得します。 |
| [getName()](#getName--) | 元のファイルの名前です。 |
| [getUncompressedSize()](#getUncompressedSize--) | 元のファイルのサイズを取得します。 |
| [open()](#open--) | アーカイブを抽出用に開き、アーカイブ内容のストリームを提供します。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 提供されたストリームにアーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 提供された宛先ファイルにアーカイブを保存します。 |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(File file)](#setSource-java.io.File-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(String path)](#setSource-java.lang.String-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


圧縮用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。

次の例はファイルを圧縮する方法を示しています。

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

このコンストラクタは解凍しません。解凍するには [open()](../../com.aspose.zip/gziparchive\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソースです。 |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


解凍用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。

ストリームからアーカイブを開き、`ByteArrayOutputStream` に抽出します。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

このコンストラクタは解凍しません。解凍するには [open()](../../com.aspose.zip/gziparchive\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソースです。 |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | アーカイブをロードするためのオプションです。 |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


解凍用に準備された新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

このコンストラクタは解凍しません。解凍するには [open()](../../com.aspose.zip/gziparchive\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパスです。 |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


新しい [GzipArchive](../../com.aspose.zip/gziparchive) クラスのインスタンスを初期化します。

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 出力先ストリーム。書き込み可能である必要があります。 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


パスで指定されたファイルにアーカイブを抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルがすでに存在する場合は上書きされます。 |

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
|  | destinationDirectory | java.lang.String | 抽出されたファイルを配置するディレクトリへのパスです。 |

ディレクトリが存在しない場合は作成されます。 |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


gzip アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - gzip アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリ。
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


元のファイルのサイズを取得します。

解凍中、このプロパティはサイズが正しくない可能性があります。非圧縮ファイルサイズが 4GB を超える場合、ヘッダーの 32 ビット制限によりこのプロパティは誤った値を返します。

**Returns:**
java.lang.Long - 元のファイルのサイズ
### getName() {#getName--}
```
public final String getName()
```


元のファイルの名前です。

**Returns:**
java.lang.String - 元のファイル名
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


元のファイルのサイズを取得します。

解凍中、このプロパティはサイズが正しくない可能性があります。非圧縮ファイルサイズが 4GB を超える場合、ヘッダーの 32 ビット制限によりこのプロパティは誤った値を返します。

**Returns:**
long - 元のファイルのサイズ。
### open() {#open--}
```
public final InputStream open()
```


アーカイブを抽出用に開き、アーカイブ内容のストリームを提供します。

アーカイブを抽出し、抽出された内容をファイルストリームにコピーします。

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | 出力先ストリームです。 |

`outputStream` は書き込み可能である必要があります。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


提供された宛先ファイルにアーカイブを保存します。

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

このメソッドを使用して結合 tar.gz アーカイブを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 圧縮される Tar アーカイブ。 |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブ用の入力ストリームです。 |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


アーカイブ内で圧縮されるコンテンツを設定します。

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

