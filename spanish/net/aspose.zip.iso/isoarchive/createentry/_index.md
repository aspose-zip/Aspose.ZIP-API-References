---
title: "IsoArchive.CreateEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método IsoArchive. Añade un archivo a la imagen ISO"
type: docs
weight: 40
url: /es/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Agrega un archivo a la imagen ISO.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | Ruta del archivo en el ISO. |
| filePath | String | Ruta del archivo. |

### Valor devuelto

La entrada ISO compuesta.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | El *filePath* es nulo. |
| ArgumentException | El *filePath* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *filePath* denegado. |
| PathTooLongException | El *filePath* especificado supera la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *filePath* contiene dos puntos (:) en medio de la cadena. |
| IOException | Se produjo un error de E/S al abrir el archivo. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| DirectoryNotFoundException | La ruta especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| FileNotFoundException | El archivo especificado en *filePath* no se encontró. |
| InvalidOperationException | El archivo no está en modo de edición. |

### Ver también

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Agrega un archivo a la imagen ISO.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | Ruta del archivo en el ISO. |
| origen | Flujo | Secuencia que contiene los datos del archivo. |

### Valor devuelto

La entrada ISO compuesta.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | Se lanza cuando *name* o *source* son nulos. |
| InvalidOperationException | El archivo no está en modo de edición. |

### Ver también

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Agrega un archivo a la imagen ISO.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | Ruta del directorio en el ISO. |

### Valor devuelto

La entrada ISO compuesta.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | `name` es null o está vacío. |
| InvalidOperationException | El archivo está abierto para extracción. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

### Ver también

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


