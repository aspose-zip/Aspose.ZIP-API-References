---
title: "Händelse"
second_title: "Aspose.ZIP för Java API-referens"
description: "En händelse."
type: docs
weight: 160
url: /sv/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

En händelse.

`TArgs`: händelseargument.

TArgs :
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Denna metod anropas när händelsen avges. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Denna metod anropas när händelsen avges.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| avsändare | java.lang.Object | ett objekt som initierar denna händelse. |
| args | TArgs | anpassade argument. |

