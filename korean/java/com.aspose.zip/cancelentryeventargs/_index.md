---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP for Java API 참조"
description: "취소 가능한 항목 관련 이벤트에 대한 이벤트 인수."
type: docs
weight: 52
url: /ko/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

취소 가능한 항목 관련 이벤트에 대한 이벤트 인수.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | 새 인스턴스를 초기화합니다 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCancel()](#getCancel--) | 이벤트를 취소해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [setCancel(boolean value)](#setCancel-boolean-) | 이벤트를 취소해야 하는지 여부를 나타내는 값을 설정합니다. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


새 인스턴스를 초기화합니다 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 클래스.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | 이벤트가 발생하는 아카이브 항목. |

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
| 값 | boolean | 이벤트를 취소해야 하면 true; 그렇지 않으면 false. |

