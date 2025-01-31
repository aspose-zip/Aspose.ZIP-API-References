---
title: CancelEntryEventArgsXar
second_title: Aspose.ZIP for Java API Reference
description: Event arguments for cancelable entry related events.
type: docs
weight: 30
url: /java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Event arguments for cancelable entry related events.
## Constructors

| Constructor | Description |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Initializes a new instance of the [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCancel()](#getCancel--) | Gets a value indicating whether the event should be canceled. |
| [setCancel(boolean value)](#setCancel-boolean-) | Sets a value indicating whether the event should be canceled. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Initializes a new instance of the [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | archive entry the event is raised for |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Gets a value indicating whether the event should be canceled.

**Returns:**
boolean - true if the event should be canceled; otherwise, false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Sets a value indicating whether the event should be canceled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true if the event should be canceled; otherwise, false |

