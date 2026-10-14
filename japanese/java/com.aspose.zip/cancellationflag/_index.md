---
title: "CancellationFlag"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "操作のキャンセルを許可するフラグ。"
type: docs
weight: 54
url: /ja/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

操作のキャンセルを許可するフラグ。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | CancellationFlag インスタンスを構築します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [cancel()](#cancel--) | この [CancellationFlag](../../com.aspose.zip/cancellationflag) インスタンスに関連付けられた操作をキャンセルします。 |
| [cancelAfter(long delay)](#cancelAfter-long-) | 指定されたミリ秒の遅延後に操作をキャンセルします。 |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | 指定された遅延時間と指定された時間単位の後に操作をキャンセルします。 |
| [close()](#close--) | [CancellationFlag](../../com.aspose.zip/cancellationflag) インスタンスを閉じ、関連するすべてのリソースを解放します。 |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


CancellationFlag インスタンスを構築します。

### cancel() {#cancel--}
```
public void cancel()
```


この [CancellationFlag](../../com.aspose.zip/cancellationflag) インスタンスに関連付けられた操作をキャンセルします。

操作がすでにキャンセルされている場合、このメソッドは何もしません。

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


指定されたミリ秒の遅延後に操作をキャンセルします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 遅延 | long | 操作がキャンセルされるまでのミリ秒単位の遅延。 |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


指定された遅延時間と指定された時間単位の後に操作をキャンセルします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 遅延 | long | 操作がキャンセルされるまでの遅延。 |
| 単位 | java.util.concurrent.TimeUnit | 遅延パラメータの時間単位。 |

### close() {#close--}
```
public void close()
```


[CancellationFlag](../../com.aspose.zip/cancellationflag) インスタンスを閉じ、関連するすべてのリソースを解放します。

