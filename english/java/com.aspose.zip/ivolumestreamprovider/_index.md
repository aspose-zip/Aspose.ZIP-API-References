---
title: IVolumeStreamProvider
second_title: Aspose.ZIP for Java API Reference
description: Provider of streams for multi-volume archive composition.
type: docs
weight: 168
url: /java/com.aspose.zip/ivolumestreamprovider/
---
```
public interface IVolumeStreamProvider
```

Provider of streams for multi-volume archive composition.
## Methods

| Method | Description |
| --- | --- |
| [getNextVolume()](#getNextVolume--) | Provides the next stream for a volume of a split archive. |
| [volumeCompleted(int index, OutputStream stream, boolean isLast)](#volumeCompleted-int-java.io.OutputStream-boolean-) | Called after a volume of a split (multi-volume) archive has been written. |
### getNextVolume() {#getNextVolume--}
```
public abstract OutputStream getNextVolume()
```


Provides the next stream for a volume of a split archive.

**Returns:**
java.io.OutputStream - the stream for the next volume.
### volumeCompleted(int index, OutputStream stream, boolean isLast) {#volumeCompleted-int-java.io.OutputStream-boolean-}
```
public abstract void volumeCompleted(int index, OutputStream stream, boolean isLast)
```


Called after a volume of a split (multi-volume) archive has been written.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the number of the volume written, starting from zero. |
| stream | java.io.OutputStream | the destination stream the volume was written to. |
| isLast | boolean | whether the volume finishes the archive. |

