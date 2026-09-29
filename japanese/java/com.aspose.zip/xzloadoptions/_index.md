---
title: "XzLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ロードのオプション。"
type: docs
weight: 152
url: /ja/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

[XzArchive](../../com.aspose.zip/xzarchive) のロードオプションです。

.NET Framework 4.0 以降では、抽出をキャンセルするために使用できます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
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
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

