---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "FastLZ でデータを圧縮するストリームラッパー。"
type: docs
weight: 68
url: /ja/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

FastLZでデータを圧縮するストリームラッパーです。デコレーターパターンを実装しています。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | 圧縮用に準備された FastLZStream クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [close()](#close--) | 現在のストリームを閉じ、現在のストリームに関連付けられたリソース（ソケットやファイルハンドルなど）を解放します。 |
| [flush()](#flush--) | このストリームのすべてのバッファをクリアし、バッファされたデータが基礎となるデバイスへ書き込まれるようにします。 |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | バイト列を書き込み、書き込まれたバイト数だけこのストリーム内の現在位置を進めます。 |
| [write(int b)](#write-int-) | 指定されたバイトをこの出力ストリームに書き込みます。 |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


圧縮用に準備された FastLZStream クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | 圧縮データを保存するストリーム |
| compressionLevel | int | 高速圧縮には 1 を、圧縮率を高めるには 2 を使用します。 |

### close() {#close--}
```
public void close()
```


現在のストリームを閉じ、現在のストリームに関連付けられたリソース（ソケットやファイルハンドルなど）を解放します。

### flush() {#flush--}
```
public void flush()
```


このストリームのすべてのバッファをクリアし、バッファされたデータが基礎となるデバイスへ書き込まれるようにします。

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


バイト列を書き込み、書き込まれたバイト数だけこのストリーム内の現在位置を進めます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| buffer | byte[] | バイトの配列です。このメソッドは buffer から現在のストリームへ count バイトをコピーします。 |
| offset | int | バッファ内のゼロベースのバイトオフセットで、ここから現在のストリームへバイトのコピーを開始します。 |
| count | int | 現在のストリームに書き込まれるバイト数 |

### write(int b) {#write-int-}
```
public void write(int b)
```


指定されたバイトをこの出力ストリームに書き込みます。`write` の一般的な契約は、1 バイトが出力ストリームに書き込まれることです。書き込まれるバイトは引数 `b` の下位 8 ビットです。`b` の上位 24 ビットは無視されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| b | int | その `byte` |

