---
title: "LzipLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ロードのオプション。"
type: docs
weight: 85
url: /ja/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

[LzipArchive](../../com.aspose.zip/lziparchive) の読み込みオプションです。

.NET Framework 4.0 以降では、抽出をキャンセルするために使用できます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。

一定時間後に lzip アーカイブの抽出をキャンセルします。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzipLoadOptions options = new LzipLoadOptions();
options.setCancellationFlag(cf);
try (LzipArchive a = new LzipArchive("big.lz", options)) {
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

