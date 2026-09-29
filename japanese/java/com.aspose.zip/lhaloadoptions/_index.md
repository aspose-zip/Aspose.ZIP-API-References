---
title: "LhaLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "圧縮ファイルからアーカイブを読み込む際のオプション。"
type: docs
weight: 78
url: /ja/java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

圧縮ファイルからアーカイブを読み込む際のオプション。

.NET Framework 4.0 以降では、抽出をキャンセルするために使用できます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。

一定時間後に LHA アーカイブの抽出をキャンセルします。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LhaLoadOptions options = new LhaLoadOptions();
options.setCancellationFlag(cf);
try (LhaArchive a = new LhaArchive("big.lha", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

