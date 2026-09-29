---
title: "Evento"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Un evento."
type: docs
weight: 160
url: /es/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Un evento.

`TArgs`: argumentos del evento.

TArgs :
## Métodos

| Método | Descripción |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Este método se invoca cuando se emite el evento. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Este método se invoca cuando se emite el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | java.lang.Object | un objeto que inicia este evento. |
| args | TArgs | argumentos personalizados. |

