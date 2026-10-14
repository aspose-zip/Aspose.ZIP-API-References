---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "LZ4 アーカイブ構成の設定。"
type: docs
weight: 81
url: /ja/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

LZ4 アーカイブ構成の設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | デフォルトパラメータで新しい [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) のインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | 圧縮ブロックの末尾に圧縮された xxh32 ハッシュを含めるかどうかを示す値を取得します。 |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | LZ4 アーカイブの末尾にコンテンツ xxh32 ハッシュを含めるかどうかを示す値を取得します。 |
| [getIncludeContentSize()](#getIncludeContentSize--) | フレームにコンテンツサイズを含めるかどうかを示す値を取得します。 |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | 圧縮ブロックの末尾に圧縮された xxh32 ハッシュを含めるかどうかを示す値を設定します。 |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | LZ4 アーカイブの末尾にコンテンツ xxh32 ハッシュを含めるかどうかを示す値を設定します。 |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | フレームにコンテンツサイズを含めるかどうかを示す値を設定します。 |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


デフォルトパラメータで新しい [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) のインスタンスを初期化します。

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


圧縮ブロックの末尾に圧縮された xxh32 ハッシュを含めるかどうかを示す値を取得します。

既定値は false です。

**Returns:**
boolean - 圧縮ブロックの末尾に圧縮された xxh32 ハッシュを含めるかどうかを示す値。
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


LZ4 アーカイブの末尾にコンテンツ xxh32 ハッシュを含めるかどうかを示す値を取得します。

既定値は true です。

**Returns:**
boolean - LZ4 アーカイブの末尾にコンテンツ xxh32 ハッシュを含めるかどうかを示す値。
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


フレームにコンテンツサイズを含めるかどうかを示す値を取得します。

既定値は false です。ソースストリームがシーク可能な場合に適用されます。

**Returns:**
boolean - フレームにコンテンツサイズを含めるかどうかを示す値。
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


圧縮ブロックの末尾に圧縮された xxh32 ハッシュを含めるかどうかを示す値を設定します。

既定値は false です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 圧縮ブロックの末尾に圧縮された xxh32 ハッシュを含めるかどうかを示す値。 |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


LZ4 アーカイブの末尾にコンテンツ xxh32 ハッシュを含めるかどうかを示す値を設定します。

既定値は true です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | LZ4 アーカイブの末尾にコンテンツ xxh32 ハッシュを含めるかどうかを示す値。 |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


フレームにコンテンツサイズを含めるかどうかを示す値を設定します。

既定値は false です。ソースストリームがシーク可能な場合に適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | フレームにコンテンツサイズを含めるかどうかを示す値。 |

