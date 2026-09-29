---
title: "Evento"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Un evento."
type: docs
weight: 160
url: /it/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Un evento.

`TArgs`: argomenti dell'evento.

TArgs :
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Questo metodo viene invocato quando l'evento viene emesso. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Questo metodo viene invocato quando l'evento viene emesso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mittente | java.lang.Object | un oggetto che avvia questo evento. |
| argomenti | TArgs | argomenti personalizzati. |

