---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "アーカイブ形式を検出し、その他の関連情報を提供します。"
type: docs
weight: 32
url: /ja/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

アーカイブ形式を検出し、その他の関連情報を提供します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | 新しい [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | フォーマット情報を取得します。 |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | フォーマット情報を取得します。 |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


新しい [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) クラスのインスタンスを初期化します。

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


フォーマット情報を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | アーカイブファイルのストリームです。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


フォーマット情報を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | アーカイブファイルのファイル名です。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
