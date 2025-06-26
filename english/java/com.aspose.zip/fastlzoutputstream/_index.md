---
title: FastLZOutputStream
second_title: Aspose.ZIP for Java API Reference
description: A stream wrapper that compresses data with FastLZ.
type: docs
weight: 46
url: /java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

A stream wrapper that compresses data with FastLZ. Implements decorator pattern.
## Constructors

| Constructor | Description |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Initializes a new instance of the FastLZStream class prepared for compression. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | Closes the current stream and releases any resources (such as sockets and file handles) associated with the current stream. |
| [flush()](#flush--) | Clears all buffers for this stream and causes any buffered data to be written to the underlying device. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Writes a sequence of bytes to the compressing stream and advances the current position within this stream by the number of bytes written. |
| [write(int b)](#write-int-) | Writes the specified byte to this output stream. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Initializes a new instance of the FastLZStream class prepared for compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream for saving compressed data |
| compressionLevel | int | use 1 for faster compression, use 2 for better compression ratio |

### close() {#close--}
```
public void close()
```


Closes the current stream and releases any resources (such as sockets and file handles) associated with the current stream.

### flush() {#flush--}
```
public void flush()
```


Clears all buffers for this stream and causes any buffered data to be written to the underlying device.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Writes a sequence of bytes to the compressing stream and advances the current position within this stream by the number of bytes written.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| buffer | byte[] | an array of bytes. This method copies count bytes from buffer to the current stream |
| offset | int | the zero-based byte offset in buffer at which to begin copying bytes to the current stream |
| count | int | the number of bytes to be written to the current stream |

### write(int b) {#write-int-}
```
public void write(int b)
```


Writes the specified byte to this output stream. The general contract for `write` is that one byte is written to the output stream. The byte to be written is the eight low-order bits of the argument `b`. The 24 high-order bits of `b` are ignored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| b | int | the `byte` |

