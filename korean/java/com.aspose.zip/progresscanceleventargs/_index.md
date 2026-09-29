---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP for Java API 참조"
description: "진행된 바이트 수를 포함하는 취소 가능한 이벤트 데이터용 클래스."
type: docs
weight: 95
url: /ko/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

진행된 바이트 수를 포함하는 취소 가능한 이벤트 데이터용 클래스.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | 새로운 [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) 클래스의 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCancel()](#getCancel--) | 이벤트를 취소해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [setCancel(boolean value)](#setCancel-boolean-) | 이벤트를 취소해야 하는지 여부를 나타내는 값을 설정합니다. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


새로운 [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) 클래스의 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| proceededBytes | long | 진행된 바이트 수. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


이벤트를 취소해야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이벤트를 취소해야 하면 true; 그렇지 않으면 false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


이벤트를 취소해야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 이벤트를 취소해야 하는지 여부를 나타내는 값. |

