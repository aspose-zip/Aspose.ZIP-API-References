---
title: "EntryEventArgsXar"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Argumentos de evento para eventos relacionados con entradas."
type: docs
weight: 64
url: /es/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

Argumentos de evento para eventos relacionados con entradas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | Inicializa una nueva instancia de la clase [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEntry()](#getEntry--) | Obtiene la entrada del archivo para la cual se genera el evento. |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


Inicializa una nueva instancia de la clase [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | la entrada del archivo para la cual se genera el evento |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


Obtiene la entrada del archivo para la cual se genera el evento.

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
