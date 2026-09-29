---
title: "AlzArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ALZ アーカイブ ファイルを表します。"
type: docs
weight: 11
url: /ja/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Represents an ALZ archive file. Use this class to inspect and extract ALZ archives.
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | ストリームから ALZ アーカイブを初期化します。 |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | 提供されたロード オプションを使用して、ストリームから ALZ アーカイブを初期化します。 |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | ファイル パスから ALZ アーカイブを初期化します。 |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | 提供されたロード オプションを使用して、ファイル パスから ALZ アーカイブを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | このアーカイブが保持するリソースを解放します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 提供されたディレクトリにすべてのファイルとディレクトリを抽出します。 |
| [getEntries()](#getEntries--) | このアーカイブを構成するエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | 共通アーカイブ インターフェイスを介してエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


ストリームから ALZ アーカイブを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ALZ アーカイブ ストリーム; 読み取りとシークをサポートしている必要があります |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


提供されたロード オプションを使用して、ストリームから ALZ アーカイブを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ALZ アーカイブ ストリーム; 読み取りとシークをサポートしている必要があります |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | アーカイブをロードするために使用されるオプション |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


ファイル パスから ALZ アーカイブを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ALZ アーカイブへのパス |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


提供されたロード オプションを使用して、ファイル パスから ALZ アーカイブを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ALZ アーカイブへのパス |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | アーカイブをロードするために使用されるオプション |

### close() {#close--}
```
public void close()
```


このアーカイブが保持するリソースを解放します。

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


提供されたディレクトリにすべてのファイルとディレクトリを抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 宛先ディレクトリ; 必要に応じて作成されます |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


このアーカイブを構成するエントリを取得します。

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - ALZ エントリの不変リスト
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


共通アーカイブ インターフェイスを介してエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - アーカイブエントリ
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


アーカイブ形式を取得します。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
