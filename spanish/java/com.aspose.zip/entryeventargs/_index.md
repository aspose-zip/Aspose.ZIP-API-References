---
title: "EntryEventArgs"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Argumentos de evento para eventos relacionados con entradas."
type: docs
weight: 62
url: /es/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Argumentos de evento para eventos relacionados con entradas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Inicializa una nueva instancia de la clase [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEntry()](#getEntry--) | Obtiene la entrada del archivo para la cual se genera el evento. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Inicializa una nueva instancia de la clase [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Entrada del archivo para la que se genera el evento. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Obtiene la entrada del archivo para la cual se genera el evento.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
