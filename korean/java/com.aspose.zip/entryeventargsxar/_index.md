---
title: "EntryEventArgsXar"
second_title: "Aspose.ZIP for Java API 참조"
description: "항목 관련 이벤트에 대한 이벤트 인수."
type: docs
weight: 64
url: /ko/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

항목 관련 이벤트에 대한 이벤트 인수.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | [ArchiveEntry](../../com.aspose.zip/entryeventargs) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getEntry()](#getEntry--) | 이벤트가 발생한 아카이브 항목을 가져옵니다. |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


[ArchiveEntry](../../com.aspose.zip/entryeventargs) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | 이벤트가 발생한 아카이브 항목 |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


이벤트가 발생한 아카이브 항목을 가져옵니다.

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
