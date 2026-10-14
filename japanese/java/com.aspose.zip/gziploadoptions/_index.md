---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ロードのオプション。"
type: docs
weight: 70
url: /ja/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

[GzipArchive](../../com.aspose.zip/gziparchive) のロードオプション。

.NET Framework 4.0 以降では、抽出をキャンセルするために使用できます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | ストリームヘッダーを解析してプロパティ（名前を含む）を取得するかどうかを示す値を取得します。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | ストリームヘッダーを解析してプロパティ（名前を含む）を取得するかどうかを示す値を設定します。 |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


ストリームヘッダーを解析してプロパティ（名前を含む）を取得するかどうかを示す値を取得します。シーク可能なストリームに対してのみ意味があります。

**Returns:**
boolean - ストリームヘッダーを解析してプロパティ（名前を含む）を取得するかどうかを示す値。
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。

一定時間後に gzip アーカイブの抽出をキャンセルします。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("抽出は60秒後にキャンセルされました");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

