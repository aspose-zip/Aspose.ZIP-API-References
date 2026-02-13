---
title: CancelEntryEventArgs
second_title: Aspose.ZIP for Java API Reference
description: Event arguments for cancelable entry related events.
type: docs
weight: 36
url: /java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Event arguments for cancelable entry related events.
## Constructors

| Constructor | Description |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initializes a new instance of the [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCancel()](#getCancel--) | Gets a value indicating whether the event should be canceled. |
| [setCancel(boolean value)](#setCancel-boolean-) | Sets a value indicating whether the event should be canceled. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Initializes a new instance of the [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Archive entry the event is raised for. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Gets a value indicating whether the event should be canceled.

**Returns:**
boolean - true if the event should be canceled; otherwise, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Sets a value indicating whether the event should be canceled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true if the event should be canceled; otherwise, false. |

