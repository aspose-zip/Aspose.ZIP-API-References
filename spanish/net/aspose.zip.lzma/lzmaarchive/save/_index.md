---
title: LzmaArchive.Save
second_title: Referencia de la API de Aspose.ZIP para .NET
description: LzmaArchive método. Guarda el archivo lzma en la secuencia proporcionada.
type: docs
weight: 40
url: /es/net/aspose.zip.lzma/lzmaarchive/save/
---
## Save(Stream) {#save_1}

Guarda el archivo lzma en la secuencia proporcionada.

```csharp
public void Save(Stream output)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| output | Stream | Flujo de destino. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *output* no admite la búsqueda. |
| ArgumentNullException | *output* es nulo. |

### Observaciones

*output* debe ser buscable.

### Ejemplos

```csharp
using (FileStream lzmaFile = File.Open("archive.lzma", FileMode.Create))
{
    using (var archive = new LzmaArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzmaFile);
     }
}
```

### Ver también

* class [LzmaArchive](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchive/)
* asamblea [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Guarda el archivo lzma en el archivo de destino proporcionado.

```csharp
public void Save(FileInfo destination)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destination | FileInfo | FileInfo que se abrirá como flujo de destino. |

### Excepciones

| excepción | condición |
| --- | --- |
| SecurityException | La persona que llama no tiene el permiso requerido para abrir el*destination*. |
| ArgumentException | La ruta del archivo está vacía o solo contiene espacios en blanco. |
| FileNotFoundException | No se encuentra el archivo. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *destination* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |

### Ejemplos

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lzma"));
}
```

### Ver también

* class [LzmaArchive](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchive/)
* asamblea [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Guarda el archivo lzma en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se va a crear. Si el nombre de archivo especificado apunta a un archivo existente, se sobrescribirá. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destinationFileName* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*destinationFileName* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*destinationFileName* es denegado. |
| PathTooLongException | El especificado*destinationFileName*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*destinationFileName* contiene dos puntos (:) en medio de la cadena. |

### Ejemplos

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lzma");
}
```

### Ver también

* class [LzmaArchive](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchive/)
* asamblea [Aspose.Zip](../../../)


