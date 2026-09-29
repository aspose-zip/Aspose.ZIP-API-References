---
title: "ZArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "圧縮ファイルからロードされる際のオプション。"
type: docs
weight: 154
url: /ja/java/com.aspose.zip/zarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveLoadOptions
```

圧縮ファイルから [ZArchive](../../com.aspose.zip/zarchive) をロードする際のオプション。抽出時に発生するイベントを含みます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ZArchiveLoadOptions()](#ZArchiveLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | いくつかのバイトが抽出されたときに発生するイベントを取得します。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出操作をキャンセルするために使用されるキャンセルフラグを設定します。 |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | いくつかのバイトが抽出されたときに発生するイベントを設定します。 |
### ZArchiveLoadOptions() {#ZArchiveLoadOptions--}
```
public ZArchiveLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


いくつかのバイトが抽出されたときに発生するイベントを取得します。

```

``````

long length = 10_000_000;
ZArchiveLoadOptions loadOptions = new ZArchiveLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZArchive archive = new ZArchive("archive.z", loadOptions);
 
```

Event sender is the [ZArchive](../../com.aspose.zip/zarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Z archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZArchiveLoadOptions options = new ZArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (ZArchive a = new ZArchive("big.z", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

キャンセルは主に一部のデータが抽出されない結果となります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 抽出操作をキャンセルするために使用されるキャンセルフラグです。 |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


いくつかのバイトが抽出されたときに発生するイベントを設定します。

```

``````

long length = 10_000_000;
ZArchiveLoadOptions loadOptions = new ZArchiveLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZArchive archive = new ZArchive("archive.z", loadOptions);
 
```

Event sender is the [ZArchive](../../com.aspose.zip/zarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

