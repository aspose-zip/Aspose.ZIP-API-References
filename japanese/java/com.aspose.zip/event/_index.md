---
title: "イベント"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "イベントです。"
type: docs
weight: 160
url: /ja/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

イベントです。

`TArgs`: イベント引数です。

TArgs :
## メソッド

| メソッド | 説明 |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | このメソッドはイベントが発行されたときに呼び出されます。 |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


このメソッドはイベントが発行されたときに呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 送信者 | java.lang.Object | このイベントを開始するオブジェクトです。 |
| 引数 | TArgs | カスタム引数です。 |

