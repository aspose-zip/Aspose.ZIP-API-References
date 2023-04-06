---
title: SharArchive.DeleteEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SharArchive método. Elimina la primera aparición de una entrada específica de la lista de entradas.
type: docs
weight: 50
url: /es/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Elimina la primera aparición de una entrada específica de la lista de entradas.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| entry | SharEntry | La entrada a eliminar de la lista de entradas. |

### Valor_devuelto

Instancia de entrada compartida.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *entry* es nulo. |

### Ejemplos

Así es como puede eliminar todas las entradas excepto la última:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Ver también

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Elimina la entrada de la lista de entradas por index.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Ver también

* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)


