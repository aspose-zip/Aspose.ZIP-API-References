---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは特定の lzip アーカイブの設定を含みます。"
type: docs
weight: 84
url: /ja/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

このクラスは特定の lzip アーカイブの設定を含みます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | 特定の辞書サイズで [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) の新しいインスタンスを初期化します。 |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | 特定の辞書サイズで [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) の新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 圧縮スレッド数を取得します。 |
| [getDictionarySize()](#getDictionarySize--) | LZMA 圧縮で使用される辞書のサイズを取得します。 |
| [getFastSpeed()](#getFastSpeed--) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 1 メガバイトに等しい）。 |
| [getFastestSpeed()](#getFastestSpeed--) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 65536 バイトに等しい）。 |
| [getHighCompression()](#getHighCompression--) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 32 メガバイトに等しい）。 |
| [getMaxMemberSize()](#getMaxMemberSize--) | lzip アーカイブ内の 1 メンバーの最大サイズ（バイト単位）を取得します。 |
| [getMaximumCompression()](#getMaximumCompression--) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 64 メガバイトに等しい）。 |
| [getNormal()](#getNormal--) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 16 メガバイトに等しい）。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 圧縮スレッド数を設定します。 |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


特定の辞書サイズで [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) の新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | int | LZMA 圧縮の辞書サイズ（バイト単位） |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


特定の辞書サイズで [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) の新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | int | LZMA 圧縮の辞書サイズ（バイト単位） |
| maxMemberSize | int | lzip アーカイブ内の 1 つのメンバーの最大サイズ（バイト単位）。デフォルト値は 60 MB です。 |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


圧縮スレッド数を取得します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。

**Returns:**
int - 圧縮スレッド数
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


LZMA 圧縮で使用される辞書のサイズを取得します。

**Returns:**
int - LZMA 圧縮で使用される辞書のサイズ
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 1 メガバイトに等しい）。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 65536 バイトに等しい）。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 32 メガバイトに等しい）。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


lzip アーカイブ内の 1 メンバーの最大サイズ（バイト単位）を取得します。

**Returns:**
long - lzip アーカイブ内の 1 つのメンバーの最大サイズ（バイト単位）
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 64 メガバイトに等しい）。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) クラスのインスタンスを取得します（LZMA フィルタで辞書サイズが 16 メガバイトに等しい）。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


圧縮スレッド数を設定します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 圧縮スレッド数 |

