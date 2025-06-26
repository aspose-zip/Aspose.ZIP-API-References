---
title: CancellationFlag
second_title: Aspose.ZIP for Java API Reference
description: The flag that allows for the cancellation of operations.
type: docs
weight: 33
url: /java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

The flag that allows for the cancellation of operations.
## Constructors

| Constructor | Description |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Constructs a CancellationFlag instance. |
## Methods

| Method | Description |
| --- | --- |
| [cancel()](#cancel--) | Cancels the operation associated with this [CancellationFlag](../../com.aspose.zip/cancellationflag) instance. |
| [cancelAfter(long delay)](#cancelAfter-long-) | Cancels the operation after a specified delay in milliseconds. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Cancels the operation after a specified delay in the given time unit. |
| [close()](#close--) | Closes the [CancellationFlag](../../com.aspose.zip/cancellationflag) instance and releases any resources associated with it. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Constructs a CancellationFlag instance.

### cancel() {#cancel--}
```
public void cancel()
```


Cancels the operation associated with this [CancellationFlag](../../com.aspose.zip/cancellationflag) instance.

If the operation is already cancelled, this method does nothing.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Cancels the operation after a specified delay in milliseconds.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| delay | long | The delay in milliseconds after which the operation will be cancelled. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Cancels the operation after a specified delay in the given time unit.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| delay | long | The delay after which the operation will be cancelled. |
| unit | java.util.concurrent.TimeUnit | The time unit of the delay parameter. |

### close() {#close--}
```
public void close()
```


Closes the [CancellationFlag](../../com.aspose.zip/cancellationflag) instance and releases any resources associated with it.

