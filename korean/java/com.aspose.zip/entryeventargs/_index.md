---
title: "EntryEventArgs"
second_title: "Aspose.ZIP for Java API 참조"
description: "항목 관련 이벤트에 대한 이벤트 인수."
type: docs
weight: 62
url: /ko/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

항목 관련 이벤트에 대한 이벤트 인수.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | [ArchiveEntry](../../com.aspose.zip/entryeventargs) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getEntry()](#getEntry--) | 이벤트가 발생한 아카이브 항목을 가져옵니다. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


[ArchiveEntry](../../com.aspose.zip/entryeventargs) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | 이벤트가 발생하는 아카이브 항목. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


이벤트가 발생한 아카이브 항목을 가져옵니다.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
