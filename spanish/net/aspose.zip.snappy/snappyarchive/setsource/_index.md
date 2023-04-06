---
title: SnappyArchive.SetSource
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SnappyArchive método. Establece el contenido que se comprimirá dentro del archivo.
type: docs
weight: 50
url: /es/net/aspose.zip.snappy/snappyarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | El flujo de entrada para el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | El*source* la corriente no se puede buscar. |

### Ejemplos

```csharp
using (var archive = new SnappyArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.snappy");
}
```

### Ver también

* class [SnappyArchive](../)
* espacio de nombres [Aspose.Zip.Snappy](../../snappyarchive/)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo que se abrirá como flujo de entrada. |

### Excepciones

| excepción | condición |
| --- | --- |
| SecurityException | La persona que llama no tiene el permiso requerido para abrir el*fileInfo*. |
| ArgumentException | La ruta del archivo está vacía o solo contiene espacios en blanco. |
| FileNotFoundException | No se encuentra el archivo. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *fileInfo* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |

### Ejemplos

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.snappy");
}
```

### Ver también

* class [SnappyArchive](../)
* espacio de nombres [Aspose.Zip.Snappy](../../snappyarchive/)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(string sourcePath)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourcePath | String | Ruta al archivo que se abrirá como flujo de entrada. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourcePath* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*sourcePath* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*sourcePath* es denegado. |
| PathTooLongException | El especificado*sourcePath*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*sourcePath* contiene dos puntos (:) en medio de la cadena. |

### Ejemplos

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### Ver también

* class [SnappyArchive](../)
* espacio de nombres [Aspose.Zip.Snappy](../../snappyarchive/)
* asamblea [Aspose.Zip](../../../)


