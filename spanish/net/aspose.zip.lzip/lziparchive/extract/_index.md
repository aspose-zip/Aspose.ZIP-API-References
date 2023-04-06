---
title: LzipArchive.Extract
second_title: Referencia de la API de Aspose.ZIP para .NET
description: LzipArchive método. Extrae el archivo lzip a una secuencia.
type: docs
weight: 40
url: /es/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

Extrae el archivo lzip a una secuencia.

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
| InvalidDataException | Error en datos en cabecera o checksum. |
| ArgumentNullException | El flujo de destino es nulo. |
| ArgumentException | El flujo de destino no admite la escritura. |

### Ejemplos

```csharp
using (FileStream sourceLzipFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new LzipArchive(sourceLzipFile))
        {
               archive.Extract(extractedFile);
           }
       }
}
```

### Ver también

* class [LzipArchive](../)
* espacio de nombres [Aspose.Zip.Lzip](../../lziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Extrae el archivo lzip a un archivo.

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
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ver también

* class [LzipArchive](../)
* espacio de nombres [Aspose.Zip.Lzip](../../lziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Extrae el archivo lzip a un archivo por ruta.

```csharp
public void Extract(string path)
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
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Ver también

* class [LzipArchive](../)
* espacio de nombres [Aspose.Zip.Lzip](../../lziparchive/)
* asamblea [Aspose.Zip](../../../)


