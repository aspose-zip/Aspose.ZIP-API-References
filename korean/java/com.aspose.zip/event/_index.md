---
title: "이벤트"
second_title: "Aspose.ZIP for Java API 참조"
description: "이벤트."
type: docs
weight: 160
url: /ko/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

이벤트.

`TArgs`: 이벤트 인수.

TArgs :
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | 이 메서드는 이벤트가 발생할 때 호출됩니다. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


이 메서드는 이벤트가 발생할 때 호출됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 보내는 객체 | java.lang.Object | 이 이벤트를 발생시키는 객체. |
| 인수 | TArgs | 사용자 지정 인수. |

