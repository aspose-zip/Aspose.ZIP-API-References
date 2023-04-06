---
title: TarArchive.DeleteEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Elimina la primera aparición de una entrada específica de la lista de entradas.
type: docs
weight: 90
url: /es/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Elimina la primera aparición de una entrada específica de la lista de entradas.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| entry | TarEntry | La entrada a eliminar de la lista de entradas. |

### Valor_devuelto

El archivo con la entrada eliminada.

### Ejemplos

Así es como puede eliminar todas las entradas excepto la última:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Ver también

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Elimina la entrada de la lista de entradas por index.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


