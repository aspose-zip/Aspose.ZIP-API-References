---
title: ArchiveLoadOptions.EntryListed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: ArchiveLoadOptions propiedad. Obtiene o establece el delegado invocado cuando aparece una entrada en la tabla de contenido.
type: docs
weight: 50
url: /es/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Obtiene o establece el delegado invocado cuando aparece una entrada en la tabla de contenido.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Ejemplos

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Ver también

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* espacio de nombres [Aspose.Zip](../../archiveloadoptions/)
* asamblea [Aspose.Zip](../../../)


