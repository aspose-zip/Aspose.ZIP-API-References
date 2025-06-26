---
title: ProgressCancelEventArgs
second_title: Aspose.ZIP for Java API Reference
description: Class for cancelable event data containing the number of bytes proceeded.
type: docs
weight: 70
url: /java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Class for cancelable event data containing the number of bytes proceeded.
## Constructors

| Constructor | Description |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Initializes a new instance of the [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCancel()](#getCancel--) | Gets a value indicating whether the event should be canceled. |
| [setCancel(boolean value)](#setCancel-boolean-) | Sets a value indicating whether the event should be canceled. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Initializes a new instance of the [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| proceededBytes | long | The number of bytes proceeded. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Gets a value indicating whether the event should be canceled.

**Returns:**
boolean - True if the event should be canceled; otherwise, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Sets a value indicating whether the event should be canceled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the event should be canceled. |

