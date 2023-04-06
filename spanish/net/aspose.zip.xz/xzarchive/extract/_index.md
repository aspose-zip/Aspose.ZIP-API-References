---
title: XzArchive.Extract
second_title: Referencia de la API de Aspose.ZIP para .NET
description: XzArchive método. Extrae el archivo xz a una secuencia.
type: docs
weight: 30
url: /es/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

Extrae el archivo xz a una secuencia.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destination | Stream | Stream para almacenar datos descomprimidos. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Los encabezados de archivo y la información de servicio no se leyeron. |

### Ejemplos

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Ver también

* class [XzArchive](../)
* espacio de nombres [Aspose.Zip.Xz](../../xzarchive/)
* asamblea [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrae el archivo xz a un archivo.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo para almacenar datos descomprimidos. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Los encabezados de archivo y la información de servicio no se leyeron. |
| SecurityException | La persona que llama no tiene el permiso requerido para abrir el*fileInfo*. |
| ArgumentException | La ruta del archivo está vacía o solo contiene espacios en blanco. |
| FileNotFoundException | No se encuentra el archivo. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *fileInfo* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |

### Ejemplos

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ver también

* class [XzArchive](../)
* espacio de nombres [Aspose.Zip.Xz](../../xzarchive/)
* asamblea [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrae el archivo xz a un archivo por ruta.

```csharp
public FileInfo Extract(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | Ruta al archivo que almacenará los datos descomprimidos. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Los encabezados de archivo y la información de servicio no se leyeron. |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Ejemplos

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Ver también

* class [XzArchive](../)
* espacio de nombres [Aspose.Zip.Xz](../../xzarchive/)
* asamblea [Aspose.Zip](../../../)


