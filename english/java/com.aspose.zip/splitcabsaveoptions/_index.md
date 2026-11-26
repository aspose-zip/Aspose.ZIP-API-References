---
title: SplitCabSaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving a multi-volume CAB archive.
type: docs
weight: 127
url: /java/com.aspose.zip/splitcabsaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitCabSaveOptions
```

Options for saving a multi-volume CAB archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [SplitCabSaveOptions(String fileName, long segmentSize)](#SplitCabSaveOptions-java.lang.String-long-) | Creates options for volumes named with a one-based number and a `.cab` extension, such as `volume1.cab` and `volume2.cab`. |
## Methods

| Method | Description |
| --- | --- |
| [getCloseEntrySource()](#getCloseEntrySource--) | Reports whether saving closes each entry's source after compression. |
| [getFileName()](#getFileName--) | Gets the common base name used to generate the numbered CAB file names. |
| [getSegmentSize()](#getSegmentSize--) | Gets the size limit used when writing each CAB volume. |
| [getSkipChecksumCalculation()](#getSkipChecksumCalculation--) | Reports whether checksum calculation is disabled for CAB data blocks. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Controls whether saving closes each entry's source as soon as its compression completes. |
| [setSkipChecksumCalculation(boolean value)](#setSkipChecksumCalculation-boolean-) | Controls whether checksums are calculated for CAB data blocks. |
### SplitCabSaveOptions(String fileName, long segmentSize) {#SplitCabSaveOptions-java.lang.String-long-}
```
public SplitCabSaveOptions(String fileName, long segmentSize)
```


Creates options for volumes named with a one-based number and a `.cab` extension, such as `volume1.cab` and `volume2.cab`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | base file name, with an optional `.cab` extension |
| segmentSize | long | maximum volume size, from 65536 to 2147483647 bytes inclusive |

### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Reports whether saving closes each entry's source after compression.

**Returns:**
boolean - `true` if entry sources are closed after compression
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Gets the common base name used to generate the numbered CAB file names.

**Returns:**
java.lang.String - the base name without the `.cab` extension
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Gets the size limit used when writing each CAB volume.

**Returns:**
long - the maximum volume size in bytes
### getSkipChecksumCalculation() {#getSkipChecksumCalculation--}
```
public final boolean getSkipChecksumCalculation()
```


Reports whether checksum calculation is disabled for CAB data blocks.

**Returns:**
boolean - `true` if checksums are skipped
### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Controls whether saving closes each entry's source as soon as its compression completes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | `true` to close entry sources after compression |

### setSkipChecksumCalculation(boolean value) {#setSkipChecksumCalculation-boolean-}
```
public final void setSkipChecksumCalculation(boolean value)
```


Controls whether checksums are calculated for CAB data blocks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | `true` to skip checksum calculation |

