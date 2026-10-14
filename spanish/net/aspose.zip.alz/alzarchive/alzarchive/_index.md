---
title: "AlzArchive.AlzArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor AlzArchive. Inicializa una nueva instancia de la clase AlzArchive a partir de un flujo"
type: docs
weight: 10
url: /es/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Inicializa una nueva instancia de la clase [`AlzArchive`](../) a partir de un flujo.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo del archivo ALZ. El flujo debe admitir lectura y búsqueda. |
| loadOptions | AlzArchiveLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | el flujo es nulo. |

### Ver también

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`AlzArchive`](../) a partir de una ruta de archivo.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | String | Ruta al archivo ALZ. |
| loadOptions | AlzArchiveLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | la ruta del archivo es nula. |
| FileNotFoundException | El archivo no existe. |

### Ver también

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


