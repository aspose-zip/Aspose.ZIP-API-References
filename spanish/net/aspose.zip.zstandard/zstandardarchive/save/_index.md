---
title: "ZstandardArchive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método ZstandardArchive. Guarda el archivo en el flujo proporcionado"
type: docs
weight: 60
url: /es/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Guarda el archivo en el flujo proporcionado.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outputStream | Flujo | Flujo de destino. |
| configuraciones | ZstandardSaveOptions | Configuraciones opcionales para la composición del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentException | *outputStream* no es escribible. |
| InvalidOperationException | No se ha proporcionado la fuente. |

## Observaciones

*outputStream* must be writable.

## Ejemplos

Escribir datos comprimidos al flujo de respuesta http.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Ver también

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| configuraciones | ZstandardSaveOptions | Configuraciones opcionales para la composición del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | *destinationFileName* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | El *destinationFileName* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *destinationFileName* denegado. |
| PathTooLongException | El *destinationFileName* especificado, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *destinationFileName* contiene dos puntos (:) en medio de la cadena. |
| Excepción | Lanzada cuando ocurre un error de tiempo de ejecución. |
| DirectoryNotFoundException | La ruta especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| IOException | Se produjo un error de E/S al abrir el archivo. |
| InvalidOperationException | No se ha proporcionado la fuente. |

## Ejemplos

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Ver también

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | FileInfo | FileInfo, que se abrirá como flujo de destino. |
| configuraciones | ZstandardSaveOptions | Configuraciones opcionales para la composición del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| SecurityException | El llamador no tiene el permiso requerido para abrir el *destino*. |
| ArgumentException | La ruta del archivo está vacía o contiene solo espacios en blanco. |
| FileNotFoundException | El archivo no se encuentra. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *destino* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| InvalidOperationException | No se ha proporcionado la fuente. |

## Ejemplos

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Ver también

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


