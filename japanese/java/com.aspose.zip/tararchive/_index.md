---
title: "TarArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは tar アーカイブファイルを表します。"
type: docs
weight: 125
url: /ja/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

このクラスは tar アーカイブファイルを表します。tar アーカイブの作成、抽出、または更新に使用します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [TarArchive()](#TarArchive--) | 新しい [TarArchive](../../com.aspose.zip/tararchive) クラスのインスタンスを初期化します。 |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | 新しい [Archive](../../com.aspose.zip/archive) クラスのインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | 新しい [TarArchive](../../com.aspose.zip/tararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | アーカイブ内に単一のエントリを作成します。 |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | エントリリストから特定のエントリの最初の出現を削除します。 |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | インデックスでエントリリストからエントリを削除します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブ内のすべてのファイルを指定されたディレクトリへ抽出します。 |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | 提供された gzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | 提供された gzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | 提供された LZ4 アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | 提供された LZ4 アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | 提供された LZMA アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | 提供された LZMA アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | 提供された lzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | 提供された lzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | 提供された xz 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromXz(String path)](#fromXz-java.lang.String-) | 提供された xz 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | 提供された Z 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromZ(String path)](#fromZ-java.lang.String-) | 提供された Z 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | 提供された Zstandard アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | 提供された Zstandard アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。 |
| [getEntries()](#getEntries--) | アーカイブを構成する [TarEntry](../../com.aspose.zip/tarentry) 型のエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | tar アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 提供されたストリームにアーカイブを保存します。 |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | 提供されたストリームにアーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 提供された宛先ファイルにアーカイブを保存します。 |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | 提供された宛先ファイルにアーカイブを保存します。 |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | gzip 圧縮でアーカイブをストリームに保存します。 |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | gzip 圧縮でアーカイブをストリームに保存します。 |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | gzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | gzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | アーカイブを LZ4 圧縮でストリームに保存します。 |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | アーカイブを LZ4 圧縮でストリームに保存します。 |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | パスで指定したファイルに LZ4 圧縮でアーカイブを保存します。 |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | パスで指定したファイルに LZ4 圧縮でアーカイブを保存します。 |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | アーカイブを LZMA 圧縮でストリームに保存します。 |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | アーカイブを LZMA 圧縮でストリームに保存します。 |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | パスで指定したファイルに lzma 圧縮でアーカイブを保存します。 |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | パスで指定したファイルに lzma 圧縮でアーカイブを保存します。 |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | lzip 圧縮でアーカイブをストリームに保存します。 |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | lzip 圧縮でアーカイブをストリームに保存します。 |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | lzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | lzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | xz 圧縮でアーカイブをストリームに保存します。 |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | xz 圧縮でアーカイブをストリームに保存します。 |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | xz 圧縮でアーカイブをストリームに保存します。 |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | xz 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | xz 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | xz 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Z 圧縮でアーカイブをストリームに保存します。 |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Z 圧縮でアーカイブをストリームに保存します。 |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Z 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Z 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Zstandard 圧縮でアーカイブをストリームに保存します。 |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Zstandard 圧縮でアーカイブをストリームに保存します。 |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Zstandard 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Zstandard 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


新しい [TarArchive](../../com.aspose.zip/tararchive) クラスのインスタンスを初期化します。

次の例はファイルを圧縮する方法を示しています。

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

このコンストラクタはエントリを展開しません。展開については [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) メソッドを参照してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソース |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


新しい [TarArchive](../../com.aspose.zip/tararchive) クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| directory | java.io.File | 圧縮するディレクトリ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 圧縮するディレクトリ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

エントリ名は `name` パラメーター内でのみ設定されます。`file` パラメーターで指定されたファイル名はエントリ名に影響しません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前 |
| ファイル | java.io.File | 圧縮対象のファイルまたはフォルダーのメタデータ |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


アーカイブ内に単一のエントリを作成します。

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

エントリ名は `name` パラメータ内でのみ設定されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前 |
| source | java.io.InputStream | エントリの入力ストリーム |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


アーカイブ内に単一のエントリを作成します。

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

エントリ名は `name` パラメーター内でのみ設定されます。`path` パラメーターで指定されたファイル名はエントリ名に影響しません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前 |
| path | java.lang.String | 圧縮するファイルへのパス |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


アーカイブ内に単一のエントリを作成します。

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | エントリリストから削除するエントリ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


インデックスでエントリリストからエントリを削除します。

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

ディレクトリが存在しない場合は、作成されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 抽出されたファイルを配置するディレクトリへのパス |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


提供された gzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: gzip アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

GZip 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソースです。 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


提供された gzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: gzip アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

GZip 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパスです。 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


提供された LZ4 アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: LZ4 アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | source | java.io.InputStream | アーカイブのソースです。 |

LZ4 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります。 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


提供された LZ4 アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: LZ4 アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | アーカイブファイルへのパスです。 |

LZ4 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります。 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


提供された LZMA アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: LZMA アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

LZMA 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


提供された LZMA アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: LZMA アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

LZMA 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


提供された lzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: lzip アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

Lzip 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソースです。 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


提供された lzip アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: lzip アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

Lzip 抽出ストリームは圧縮アルゴリズムの性質上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパスです。 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


提供された xz 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: xz アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


提供された xz 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: xz アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを操作する必要があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


提供された Z 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: Z アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


提供された Z 形式のアーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: Z アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


提供された Zstandard アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: Zstandard アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | java.io.InputStream | アーカイブのソース |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


提供された Zstandard アーカイブを抽出し、抽出データから [TarArchive](../../com.aspose.zip/tararchive) を作成します。

重要: Zstandard アーカイブはこのメソッド内で完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへのパス |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


アーカイブを構成する [TarEntry](../../com.aspose.zip/tarentry) 型のエントリを取得します。

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - アーカイブを構成する [TarEntry](../../com.aspose.zip/tarentry) 型のエントリ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


tar アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - tar アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 型のエントリ
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


アーカイブ形式を取得します。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


提供されたストリームにアーカイブを保存します。

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 宛先ストリーム。 |

`output` は書き込み可能である必要があります |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


提供された宛先ファイルにアーカイブを保存します。

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

アーカイブを読み込んだのと同じパスに保存することは可能です。ただし、この方法は一時ファイルへのコピーを使用するため推奨されません

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 作成するアーカイブのパスです。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


gzip 圧縮でアーカイブをストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 宛先ストリーム。 |

`output` は書き込み可能である必要があります |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


gzip 圧縮でパスで指定されたファイルにアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


アーカイブを LZ4 圧縮でストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | java.io.OutputStream | 出力先ストリームです。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合、USTar として扱われます。 |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


パスで指定したファイルに LZ4 圧縮でアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成されるアーカイブのパスです。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合、USTar として扱われます。 |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


アーカイブを LZMA 圧縮でストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

重要: このメソッド内で tar アーカイブが作成され、その後圧縮されます。内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 宛先ストリーム。 |

`output` は書き込み可能である必要があります |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


パスで指定したファイルに lzma 圧縮でアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

重要: このメソッド内で tar アーカイブが作成され、その後圧縮されます。内容は内部に保持されます。メモリ使用量に注意してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


lzip 圧縮でアーカイブをストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 宛先ストリーム。 |

`output` は書き込み可能である必要があります |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


lzip 圧縮でパスで指定されたファイルにアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


xz 圧縮でアーカイブをストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 宛先ストリーム。 |

`output`ストリームは書き込み可能である必要があります |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


xz 圧縮でアーカイブをストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


xz 圧縮でパスで指定されたファイルにアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Z 圧縮でアーカイブをストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | java.io.OutputStream | 宛先ストリーム |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Z 圧縮でパスで指定されたファイルにアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Zstandard 圧縮でアーカイブをストリームに保存します。

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 宛先ストリーム。 |

`output` は書き込み可能である必要があります |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Zstandard 圧縮でパスで指定されたファイルにアーカイブを保存します。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、そのファイルは上書きされます。 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar ヘッダー形式を定義します。null 値は可能な場合 USTar として扱われます |

