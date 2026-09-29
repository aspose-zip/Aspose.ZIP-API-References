---
title: "Событие"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Событие."
type: docs
weight: 160
url: /ru/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Событие.

`TArgs`: аргументы события.

TArgs :
## Методы

| Метод | Описание |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Этот метод вызывается, когда событие генерируется. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Этот метод вызывается, когда событие генерируется.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sender | java.lang.Object | объект, инициирующий это событие. |
| args | TArgs | пользовательские аргументы. |

