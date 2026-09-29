---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "マルチボリューム 7-zip アーカイブを保存するためのオプション。"
type: docs
weight: 123
url: /ja/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

マルチボリューム 7-zip アーカイブを保存するためのオプション。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | マルチボリューム 7z アーカイブの保存設定をインスタンス化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFileName()](#getFileName--) | 拡張子なしでセグメントの名前を取得します。 |
| [getSegmentSize()](#getSegmentSize--) | セグメントのサイズを取得します。 |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


マルチボリューム 7z アーカイブの保存設定をインスタンス化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | fileName | java.lang.String | ボリュームの名前。.7z 拡張子が付いていても付いていなくてもかまいません。 |

ファイル名は次のようになります: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | ボリュームのサイズ。 |

一部のボリュームは `segmentSize` 未満になる場合があります。ほとんどの場合、最後のセグメントが小さくなりますが、まれに通常のセグメントがそれより小さくなることがあります。 |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


拡張子なしでセグメントの名前を取得します。

**Returns:**
java.lang.String - 拡張子なしのセグメント名
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


セグメントのサイズを取得します。

**Returns:**
long - セグメントのサイズ。
