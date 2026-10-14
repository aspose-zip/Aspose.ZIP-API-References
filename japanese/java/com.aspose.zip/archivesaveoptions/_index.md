---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブを保存するためのオプション。"
type: docs
weight: 36
url: /ja/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

ZIP アーカイブを保存するためのオプション。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip ファイルのオプションコメントを取得します。 |
| [getCloseEntrySource()](#getCloseEntrySource--) | エントリが圧縮された直後にエントリのソースを閉じるかどうかを示す値を取得します。 |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | データディスクリプタの出力設定を取得します。 |
| [getEncoding()](#getEncoding--) | ファイル名やその他の文字列をバイトに変換するためのエンコーディングを取得します。 |
| [getEncryptionOptions()](#getEncryptionOptions--) | 既存の ZIP アーカイブを保存するための暗号化設定を取得します。 |
| [getEventsBag()](#getEventsBag--) | アーカイブ保存時に発生するイベントのコンテナを取得します。 |
| [getParallelOptions()](#getParallelOptions--) | 並列圧縮の設定を取得します。 |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | 自己解凍アーカイブの設定を取得します。 |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip ファイルのオプションコメントを設定します。 |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | エントリのソースをエントリが圧縮された直後に閉じるかどうかを示す値を設定します。 |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | データディスクリプタの出力に関する設定を行います。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | ファイル名やその他の文字列をバイトに変換するためのエンコーディングを設定します。 |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | 既存の ZIP アーカイブを保存するための暗号化設定を行います。 |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | アーカイブ保存時に発生するイベントのコンテナを設定します。 |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | 並列圧縮に関する設定を行います。 |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | 自己抽出アーカイブに関する設定を行います。 |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip ファイルのオプションコメントを取得します。

**Returns:**
java.lang.String - Zip ファイルのオプションコメントです。
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


エントリが圧縮された直後にエントリのソースを閉じるかどうかを示す値を取得します。

**Returns:**
boolean - エントリのソースをエントリが圧縮された直後に閉じるかどうかを示す値です。
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


データディスクリプタの出力設定を取得します。

デフォルトオプションは常にデータディスクリプタが存在します。

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


ファイル名やその他の文字列をバイトに変換するためのエンコーディングを取得します。

設定しない場合、コードページ 437 が使用されます。

**Returns:**
java.nio.charset.Charset - ファイル名やその他の文字列をバイトに変換するためのエンコーディングです。
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


既存の ZIP アーカイブを保存するための暗号化設定を取得します。

```

``````

try (Archive archive = new Archive(\"plain.zip\")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings(\"p@s$\", EncryptionMethod.AES256));
archive.save(\"encripted.zip\", options);
}
 
```

Do not use this options for regular composition of encrypted archive, use

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) instead.

Not compatible with `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) having value [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing ZIP archive.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### getSelfExtractorOptions() {#getSelfExtractorOptions--}
```
public final SelfExtractorOptions getSelfExtractorOptions()
```


Gets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Returns:**
[SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) - settings for self extracted archive.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Sets a value indicating whether entries' sources should be closed right after an entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether entries' sources should be closed right after an entry has been compressed. |

### setDataDescriptorPolicy(ZipDataDescriptorPolicy value) {#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-}
```
public final void setDataDescriptorPolicy(ZipDataDescriptorPolicy value)
```


Sets settings for Data Descriptor emission.

Default option is always present data descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) | settings for Data Descriptor emission. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEncryptionOptions(EncryptionSettings value) {#setEncryptionOptions-com.aspose.zip.EncryptionSettings-}
```
public final void setEncryptionOptions(EncryptionSettings value)
```


Sets encryption settings for saving existing ZIP archive.

```

``````

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

このオプションは暗号化アーカイブの通常の作成には使用しないで、代わりに使用してください

代わりに `new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) を使用してください。

`DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) と互換性がなく、値が [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) である場合

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | 既存のZIPアーカイブを保存するための暗号化設定です。 |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


アーカイブ保存時に発生するイベントのコンテナを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | アーカイブ保存時に発生するイベントのコンテナです。 |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


並列圧縮に関する設定を行います。

複数のアーカイブエントリを圧縮する際に、複数のCPUコアを利用したい場合はこれを割り当てます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | 並列圧縮の設定です。 |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


自己抽出アーカイブに関する設定を行います。

対象コンピュータにソフトウェアがインストールされていなくてもアーカイブを抽出できる実行可能プログラムを作成する必要がある場合は、これを割り当てます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | 自己抽出アーカイブの設定です。 |

