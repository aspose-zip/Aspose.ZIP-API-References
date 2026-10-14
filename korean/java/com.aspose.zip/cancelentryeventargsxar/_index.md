---
title: "CancelEntryEventArgsXar"
second_title: "Aspose.ZIP for Java API 참조"
description: "취소 가능한 항목 관련 이벤트에 대한 이벤트 인수."
type: docs
weight: 53
url: /ko/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

취소 가능한 항목 관련 이벤트에 대한 이벤트 인수.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | 새 인스턴스를 초기화합니다 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCancel()](#getCancel--) | 이벤트를 취소해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [setCancel(boolean value)](#setCancel-boolean-) | 이벤트를 취소해야 하는지 여부를 나타내는 값을 설정합니다. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


새 인스턴스를 초기화합니다 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 클래스.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | 이벤트가 발생하는 아카이브 항목 |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


이벤트를 취소해야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이벤트를 취소해야 하면 true; 그렇지 않으면 false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


이벤트를 취소해야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 이벤트를 취소해야 하면 true; 그렇지 않으면 false |

