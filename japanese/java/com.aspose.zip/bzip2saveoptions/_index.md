---
title: "Bzip2SaveOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "bzip2 アーカイブを保存するためのオプション。"
type: docs
weight: 43
url: /ja/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

bzip2 アーカイブを保存するためのオプション。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | 新しいインスタンスを初期化します。[Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) クラス。 |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | デフォルトのブロックサイズ（9 百キロバイト）で [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ブロックサイズ（百キロバイト単位）。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 生ストリームの一部が圧縮されたときに発生するイベントを取得します。 |
| [getCompressionThreads()](#getCompressionThreads--) | 圧縮スレッド数を取得します。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 生ストリームの一部が圧縮されたときに発生するイベントを設定します。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 圧縮スレッド数を設定します。 |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


新しいインスタンスを初期化します。[Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) クラス。

```

``````

try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save(result, new Bzip2SaveOptions(9));
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2SaveOptions() {#Bzip2SaveOptions--}
```
public Bzip2SaveOptions()
```


Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
         try (Bzip2Archive archive = new Bzip2Archive()) {
             archive.setSource("data.bin");
             archive.save(result, new Bzip2SaveOptions());
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


ブロックサイズ（百キロバイト単位）。

**Returns:**
int - ブロックサイズ（百キロバイト単位）
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


生ストリームの一部が圧縮されたときに発生するイベントを取得します。

```

``````

File source = new File("huge.bin");
Bzip2SaveOptions settings = new Bzip2SaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```

This event won't be raised when compressing in multithreaded mode.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     Bzip2SaveOptions settings = new Bzip2SaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```

このイベントはマルチスレッドモードで圧縮する場合には発生しません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 生ストリームの一部が圧縮されたときに発生するイベント |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


圧縮スレッド数を設定します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 圧縮スレッド数。 |

