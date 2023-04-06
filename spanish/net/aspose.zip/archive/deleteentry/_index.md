---
title: Archive.DeleteEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Archive método. Elimina la primera aparición de una entrada específica de la lista de entradas.
type: docs
weight: 60
url: /es/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Elimina la primera aparición de una entrada específica de la lista de entradas.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| entry | ArchiveEntry | La entrada a eliminar de la lista de entradas. |

### Valor_devuelto

El archivo con la entrada eliminada.

### Ejemplos

Así es como puede eliminar todas las entradas excepto la última:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Ver también

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Elimina la entrada de la lista de entradas por index.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| entryIndex | Int32 | El índice de base cero de la entrada que se va a quitar. |

### Valor_devuelto

El archivo con la entrada eliminada.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* es menor que 0.-o-*entryIndex* es igual o mayor que`Entradas` contar. |

### Ejemplos

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Ver también

* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)


