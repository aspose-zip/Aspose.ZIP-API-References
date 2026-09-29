---
title: "Ereignis"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ein Ereignis."
type: docs
weight: 160
url: /de/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Ein Ereignis.

`TArgs`: Ereignisargumente.

TArgs :
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Diese Methode wird aufgerufen, wenn das Ereignis ausgelöst wird. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Diese Methode wird aufgerufen, wenn das Ereignis ausgelöst wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Absender | java.lang.Object | ein Objekt, das dieses Ereignis auslöst. |
| Argumente | TArgs | benutzerdefinierte Argumente. |

