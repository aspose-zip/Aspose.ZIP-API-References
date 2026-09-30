---
title: "EggArchive.EggArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor EggArchive. Inicializa una nueva instancia de la clase EggArchive a partir de un flujo"
type: docs
weight: 10
url: /es/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Inicializa una nueva instancia de la clase [`EggArchive`](../) a partir de un flujo.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo del archivo EGG. El flujo debe admitir lectura y búsqueda. |
| loadOptions | EggArchiveLoadOptions | Opciones para cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *stream* es nulo. |
| ArgumentException | *stream* no es legible y buscable. |

### Ver también

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`EggArchive`](../) a partir de una ruta de archivo.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | Ruta al archivo EGG. |
| loadOptions | EggArchiveLoadOptions | Opciones para cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| FileNotFoundException | El archivo no existe. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| FileNotFoundException | El archivo no se encuentra. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |

### Ver también

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


