---
title: "ZstandardSaveOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZStandard アーカイブの設定です。"
type: docs
weight: 159
url: /ja/java/com.aspose.zip/zstandardsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardSaveOptions
```

ZStandard アーカイブの設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ZstandardSaveOptions()](#ZstandardSaveOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | 生ストリームの一部が圧縮されたときに発生するイベントを取得します。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 生ストリームの一部が圧縮されたときに発生するイベントを設定します。 |
### ZstandardSaveOptions() {#ZstandardSaveOptions--}
```
public ZstandardSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


生ストリームの一部が圧縮されたときに発生するイベントを取得します。

```

``````

File source = new File("huge.bin");
ZstandardSaveOptions settings = new ZstandardSaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     ZstandardSaveOptions settings = new ZstandardSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 生ストリームの一部が圧縮されたときに発生するイベント |

