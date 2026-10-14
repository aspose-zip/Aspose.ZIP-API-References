---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "マルチボリューム ZIP アーカイブを保存するためのオプション。"
type: docs
weight: 122
url: /ja/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

マルチボリューム ZIP アーカイブを保存するためのオプション。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | マルチボリューム ZIP アーカイブを保存するための設定をインスタンス化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip ファイルのオプションコメントを取得します。 |
| [getCloseEntrySource()](#getCloseEntrySource--) | エントリが圧縮された直後にエントリのソースを閉じるかどうかを示す値を取得します。 |
| [getEncoding()](#getEncoding--) | ファイル名やその他の文字列をバイトに変換するためのエンコーディングを取得します。 |
| [getEventsBag()](#getEventsBag--) | アーカイブ保存時に発生するイベントのコンテナを取得します。 |
| [getFileName()](#getFileName--) | 拡張子なしでセグメントの名前を取得します。 |
| [getSegmentSize()](#getSegmentSize--) | セグメントのサイズを取得します。 |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip ファイルのオプションコメントを設定します。 |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | エントリのソースをエントリが圧縮された直後に閉じるかどうかを示す値を設定します。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | ファイル名やその他の文字列をバイトに変換するためのエンコーディングを設定します。 |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | アーカイブ保存時に発生するイベントのコンテナを設定します。 |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


マルチボリューム ZIP アーカイブを保存するための設定をインスタンス化します。

一部のボリュームは `segmentSize` 未満になることがあります。ほとんどの場合、最後のセグメントが小さくなりますが、稀に通常のセグメントがそれより小さくなることがあります。

ファイル名は次のようになります: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | ボリュームの名前です。.zip 拡張子の有無にかかわらず指定できます。 |
| segmentSize | long | ボリュームのサイズ。 |

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
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


ファイル名やその他の文字列をバイトに変換するためのエンコーディングを取得します。

設定しない場合、コードページ 437 が使用されます。

**Returns:**
java.nio.charset.Charset - ファイル名やその他の文字列をバイトに変換するためのエンコーディングです。
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


アーカイブ保存時に発生するイベントのコンテナを取得します。

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


拡張子なしでセグメントの名前を取得します。

**Returns:**
java.lang.String - 拡張子なしでセグメントの名前。
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


セグメントのサイズを取得します。

**Returns:**
long - セグメントのサイズ。
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Zip ファイルのオプションコメントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Zip ファイルのオプションコメント。 |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


エントリのソースをエントリが圧縮された直後に閉じるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | エントリが圧縮された直後にエントリのソースを閉じるかどうかを示す値。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


ファイル名やその他の文字列をバイトに変換するためのエンコーディングを設定します。

設定しない場合、コードページ 437 が使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.nio.charset.Charset | ファイル名やその他の文字列をバイトに変換するためのエンコーディング。 |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


アーカイブ保存時に発生するイベントのコンテナを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | アーカイブ保存時に発生するイベントのコンテナです。 |

