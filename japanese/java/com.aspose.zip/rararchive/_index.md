---
title: "RarArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは RAR アーカイブ ファイルを表します。"
type: docs
weight: 97
url: /ja/java/com.aspose.zip/rararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class RarArchive implements IArchive, AutoCloseable
```

このクラスは RAR アーカイブファイルを表します。RAR アーカイブの抽出に使用します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [RarArchive(String path)](#RarArchive-java.lang.String-) | 新しい [RarArchive](../../com.aspose.zip/rararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [RarArchive(String path, RarArchiveLoadOptions loadOptions)](#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-) | 新しい [RarArchive](../../com.aspose.zip/rararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [RarArchive(InputStream sourceStream)](#RarArchive-java.io.InputStream-) | 新しい [RarArchive](../../com.aspose.zip/rararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)](#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-) | 新しい [RarArchive](../../com.aspose.zip/rararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブ内のすべてのファイルを指定されたディレクトリへ抽出します。 |
| [getEntries()](#getEntries--) | RAR アーカイブを構成する [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) 型のエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | RAR アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
### RarArchive(String path) {#RarArchive-java.lang.String-}
```
public RarArchive(String path)
```


新しい [RarArchive](../../com.aspose.zip/rararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

次の例ではアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (RarArchive archive = new RarArchive("data.rar")) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### RarArchive(String path, RarArchiveLoadOptions loadOptions) {#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(String path, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (RarArchive archive = new RarArchive("data.rar")) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

このコンストラクタはエントリを解凍しません。解凍するには [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### RarArchive(InputStream sourceStream) {#RarArchive-java.io.InputStream-}
```
public RarArchive(InputStream sourceStream)
```


新しい [RarArchive](../../com.aspose.zip/rararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。


以下の例は最初のエントリを復号し、`MemoryStream` に解凍します。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions) {#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.


The following example decipher and decompress first entry to a `MemoryStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (RarArchive archive = new RarArchive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

このコンストラクタはエントリを解凍しません。解凍するには [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソースです。 |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


アーカイブ内のすべてのファイルを指定されたディレクトリへ抽出します。

```

``````

try (RarArchive archive = new RarArchive("archive.rar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<RarArchiveEntry> getEntries()
```


Gets entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.

**Returns:**
java.util.List&lt;com.aspose.zip.RarArchiveEntry&gt; - entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
