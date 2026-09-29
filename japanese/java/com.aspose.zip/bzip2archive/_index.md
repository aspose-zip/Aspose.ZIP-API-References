---
title: "Bzip2Archive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは bzip2 アーカイブ ファイルを表します。"
type: docs
weight: 40
url: /ja/java/com.aspose.zip/bzip2archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Bzip2Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

このクラスは bzip2 アーカイブファイルを表します。bzip2 アーカイブの作成や抽出に使用します。

bzip2 は Burrows-Wheeler ブロックソートテキスト圧縮アルゴリズムとハフマン符号化を使用してファイルを圧縮します。詳しくは: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Bzip2Archive()](#Bzip2Archive--) | 圧縮用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。 |
| [Bzip2Archive(InputStream sourceStream)](#Bzip2Archive-java.io.InputStream-) | 解凍用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。 |
| [Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-) | 解凍用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。 |
| [Bzip2Archive(String path)](#Bzip2Archive-java.lang.String-) | 解凍用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。 |
| [Bzip2Archive(String path, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-) | 解凍用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 提供されたストリームへアーカイブを抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | パスで指定されたファイルにアーカイブを抽出します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブの内容を指定されたディレクトリに抽出します。 |
| [getFileEntries()](#getFileEntries--) | bzip2 アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getLength()](#getLength--) | 長さを取得します。 |
| [getName()](#getName--) | 元のファイル名。 |
| [open()](#open--) | アーカイブを抽出用に開き、アーカイブ内容のストリームを提供します。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 提供されたストリームにアーカイブを保存します。 |
| [save(OutputStream outputStream, Bzip2SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-) | 提供されたストリームにアーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 提供された宛先ファイルにアーカイブを保存します。 |
| [save(String destinationFileName, Bzip2SaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-) | 提供された宛先ファイルにアーカイブを保存します。 |
| [setSource(CpioArchive cpioArchive)](#setSource-com.aspose.zip.CpioArchive-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(CpioArchive cpioArchive, CpioFormat format)](#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(File file)](#setSource-java.io.File-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
| [setSource(String path)](#setSource-java.lang.String-) | アーカイブ内で圧縮されるコンテンツを設定します。 |
### Bzip2Archive() {#Bzip2Archive--}
```
public Bzip2Archive()
```


圧縮用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。

次の例はファイルを圧縮する方法を示しています。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save("archive.bz2");
}
 
```



### Bzip2Archive(InputStream sourceStream) {#Bzip2Archive-java.io.InputStream-}
```
public Bzip2Archive(InputStream sourceStream)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

このコンストラクタは解凍しません。解凍するには [open()](../../com.aspose.zip/bzip2archive\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソース |

### Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)
```


解凍用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。

ストリームからアーカイブを開き、`ByteArrayOutputStream` に抽出します。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

### Bzip2Archive(String path) {#Bzip2Archive-java.lang.String-}
```
public Bzip2Archive(String path)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

このコンストラクタは解凍しません。解凍するには [open()](../../com.aspose.zip/bzip2archive\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |

### Bzip2Archive(String path, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(String path, Bzip2LoadOptions loadOptions)
```


解凍用に準備された [Bzip2Archive](../../com.aspose.zip/bzip2archive) クラスの新しいインスタンスを初期化します。

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

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

     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | java.io.OutputStream | 宛先ストリーム。書き込み可能である必要があります。 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


パスで指定されたファイルにアーカイブを抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |

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


bzip2 アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - bzip2 アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリ
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
### open() {#open--}
```
public final InputStream open()
```


アーカイブを抽出用に開き、アーカイブ内容のストリームを提供します。


使用方法:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to an output stream.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outputStream | java.io.OutputStream | 宛先ストリーム。 |

### save(OutputStream outputStream, Bzip2SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(OutputStream outputStream, Bzip2SaveOptions saveOptions)
```


提供されたストリームにアーカイブを保存します。

圧縮データを出力ストリームに書き込みます。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream. |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

Writes compressed data to file.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bz2");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |

### save(String destinationFileName, Bzip2SaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(String destinationFileName, Bzip2SaveOptions saveOptions)
```


提供された宛先ファイルにアーカイブを保存します。

圧縮データをファイルに書き込みます。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File("data.bin"));
archive.save("data.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### setSource(CpioArchive cpioArchive) {#setSource-com.aspose.zip.CpioArchive-}
```
public final void setSource(CpioArchive cpioArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (CpioArchive cpioArchive = new CpioArchive()) {
         cpioArchive.createEntry("first.bin", "data1.bin");
         cpioArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(cpioArchive);
             bzippedArchive.save("archive.cpio.bz2");
         }
     }
 
```

このメソッドを使用して結合 cpio.bz2 アーカイブを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | 圧縮対象の cpio アーカイブ |

### setSource(CpioArchive cpioArchive, CpioFormat format) {#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-}
```
public final void setSource(CpioArchive cpioArchive, CpioFormat format)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (CpioArchive cpioArchive = new CpioArchive()) {
cpioArchive.createEntry("first.bin", "data1.bin");
cpioArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(cpioArchive);
bzippedArchive.save("archive.cpio.bz2");
}
}
 
```

Use this method to compose joint cpio.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio archive to be compressed |
| format | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

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
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(tarArchive);
             bzippedArchive.save("archive.tar.bz2");
         }
     }
 
```

このメソッドを使用して結合 tar.bz2 アーカイブを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 圧縮対象の tar アーカイブ |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(tarArchive);
bzippedArchive.save("archive.tar.bz2");
}
}
 
```

Use this method to compose joint tar.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar archive to be compressed |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル | java.io.File | 圧縮対象ファイルへの参照 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


アーカイブ内で圧縮されるコンテンツを設定します。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 圧縮するファイルへのパス |

