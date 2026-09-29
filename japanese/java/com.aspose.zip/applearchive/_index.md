---
title: "AppleArchive"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは Apple Archive の .aar ファイルを表します。"
type: docs
weight: 16
url: /ja/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

このクラスは Apple Archive（.aar）ファイルを表します。Apple Archive ファイルを作成するために使用します。

Apple と Apple Archive は Apple Inc. の商標です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | 作成されたエントリで使用される設定を持つ [AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。 |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | 作成されたエントリで使用される設定を持つ [AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。 |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。 |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。 |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。 |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | アーカイブ内に単一のエントリを作成します。 |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | アーカイブ内に単一のエントリを作成します。 |
| [dispose()](#dispose--) | アンマネージ リソースの解放、リリース、またはリセットに関連するアプリケーション定義タスクを実行します。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | アーカイブ内のすべてのファイルを指定されたディレクトリへ抽出します。 |
| [getEntries()](#getEntries--) | アーカイブを構成するエントリを取得します。 |
| [getFileEntries()](#getFileEntries--) | アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) タイプのエントリを取得します。 |
| [getFormat()](#getFormat--) | アーカイブ形式を取得します。 |
| [getNewEntrySettings()](#getNewEntrySettings--) | 新しく作成されたエントリで使用される設定を取得します。 |
| [isSolid()](#isSolid--) | アーカイブがソリッド圧縮を使用しているかどうかを示す値を取得します。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 提供されたストリームにアーカイブを保存します。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 指定された宛先ファイルにアーカイブを保存します。 |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


作成されたエントリで使用される設定を持つ [AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


作成されたエントリで使用される設定を持つ [AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | 新しい Apple Archive を作成する際に使用される設定。 |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | アーカイブのソースです。 |

このコンストラクタはエントリを展開しません。展開については [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) と [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) メソッドを参照してください。 |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | アーカイブのソースです。 |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

このコンストラクタはエントリを展開しません。展開については [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) と [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) メソッドを参照してください。 |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |

このコンストラクタはエントリを展開しません。展開については [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) と [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) メソッドを参照してください。 |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


アーカイブから抽出できるエントリリストを作成し、[AppleArchive](../../com.aspose.zip/applearchive) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | 既存のアーカイブをロードするためのオプションです。 |

このコンストラクタはエントリを展開しません。展開については [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) と [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) メソッドを参照してください。 |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| directory | java.io.File | 圧縮するディレクトリ。 |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| directory | java.io.File | 圧縮するディレクトリ。 |
| includeRootDirectory | boolean | ルートディレクトリ自体を含めるかどうかを示します。 |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


アーカイブ内に単一のエントリを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前。 |
| fileInfo | java.io.File | 圧縮対象ファイルのメタデータ。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


アーカイブ内に単一のエントリを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前。 |
| fileInfo | java.io.File | 圧縮対象ファイルのメタデータ。 |
| openImmediately | boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


アーカイブ内に単一のエントリを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前。 |
| source | java.io.InputStream | エントリ用の入力ストリーム。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


アーカイブ内に単一のエントリを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前。 |
| path | java.lang.String | 圧縮するファイルへのパス。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


アーカイブ内に単一のエントリを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String | エントリの名前。 |
| path | java.lang.String | 圧縮するファイルへのパス。 |
| openImmediately | boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


アンマネージ リソースの解放、リリース、またはリセットに関連するアプリケーション定義タスクを実行します。

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


アーカイブ内のすべてのファイルを指定されたディレクトリへ抽出します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 抽出されたファイルを配置するディレクトリへのパスです。 |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


アーカイブを構成するエントリを取得します。

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - アーカイブを構成するエントリ。
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


アーカイブを構成する [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) タイプのエントリを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - アーカイブを構成する[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)型のエントリ
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


アーカイブ形式を取得します。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


新しく作成されたエントリで使用される設定を取得します。

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


アーカイブがソリッド圧縮を使用しているかどうかを示す値を取得します。ソリッドモードでは、すべてのエントリデータが単一のストリームとして圧縮され、個別のエントリ抽出は利用できません。代わりに[IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--)を使用してください。

**Returns:**
boolean - アーカイブがソリッド圧縮を使用しているかどうかを示す値。
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


提供されたストリームにアーカイブを保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | output | java.io.OutputStream | 出力先ストリームです。 |

`output` は書き込み可能である必要があります。LZ4 などの圧縮設定では、シーク可能なストリームが必要になる場合があります。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


指定された宛先ファイルにアーカイブを保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 作成するアーカイブのパス。 |

