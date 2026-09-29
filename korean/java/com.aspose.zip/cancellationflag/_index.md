---
title: "CancellationFlag"
second_title: "Aspose.ZIP for Java API 참조"
description: "작업 취소를 허용하는 플래그."
type: docs
weight: 54
url: /ko/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

작업 취소를 허용하는 플래그.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | CancellationFlag 인스턴스를 생성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [cancel()](#cancel--) | 이 [CancellationFlag](../../com.aspose.zip/cancellationflag) 인스턴스와 연결된 작업을 취소합니다. |
| [cancelAfter(long delay)](#cancelAfter-long-) | 지정된 밀리초 지연 후 작업을 취소합니다. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | 지정된 시간 단위의 지연 후 작업을 취소합니다. |
| [close()](#close--) | [CancellationFlag](../../com.aspose.zip/cancellationflag) 인스턴스를 닫고 이에 연결된 모든 리소스를 해제합니다. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


CancellationFlag 인스턴스를 생성합니다.

### cancel() {#cancel--}
```
public void cancel()
```


이 [CancellationFlag](../../com.aspose.zip/cancellationflag) 인스턴스와 연결된 작업을 취소합니다.

작업이 이미 취소된 경우, 이 메서드는 아무 작업도 수행하지 않습니다.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


지정된 밀리초 지연 후 작업을 취소합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| delay | long | 작업이 취소되는 밀리초 단위의 지연. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


지정된 시간 단위의 지연 후 작업을 취소합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| delay | long | 작업이 취소되는 지연 시간. |
| unit | java.util.concurrent.TimeUnit | 지연 매개변수의 시간 단위입니다. |

### close() {#close--}
```
public void close()
```


[CancellationFlag](../../com.aspose.zip/cancellationflag) 인스턴스를 닫고 이에 연결된 모든 리소스를 해제합니다.

