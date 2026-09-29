---
title: "CancellationFlag"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Флаг, позволяющий отменять операции."
type: docs
weight: 54
url: /ru/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Флаг, позволяющий отменять операции.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Создаёт экземпляр CancellationFlag. |
## Методы

| Метод | Описание |
| --- | --- |
| [cancel()](#cancel--) | Отменяет операцию, связанную с этим экземпляром [CancellationFlag](../../com.aspose.zip/cancellationflag). |
| [cancelAfter(long delay)](#cancelAfter-long-) | Отменяет операцию после указанной задержки в миллисекундах. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Отменяет операцию после указанной задержки в заданной единице времени. |
| [close()](#close--) | Закрывает экземпляр [CancellationFlag](../../com.aspose.zip/cancellationflag) и освобождает любые связанные с ним ресурсы. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Создаёт экземпляр CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


Отменяет операцию, связанную с этим экземпляром [CancellationFlag](../../com.aspose.zip/cancellationflag).

Если операция уже отменена, этот метод ничего не делает.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Отменяет операцию после указанной задержки в миллисекундах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| delay | long | Задержка в миллисекундах, после которой операция будет отменена. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Отменяет операцию после указанной задержки в заданной единице времени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| delay | long | Задержка, после которой операция будет отменена. |
| unit | java.util.concurrent.TimeUnit | Единица измерения времени параметра задержки. |

### close() {#close--}
```
public void close()
```


Закрывает экземпляр [CancellationFlag](../../com.aspose.zip/cancellationflag) и освобождает любые связанные с ним ресурсы.

