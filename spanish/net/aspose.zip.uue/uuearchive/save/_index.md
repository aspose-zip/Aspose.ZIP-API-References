---
title: "UueArchive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método UueArchive. Guarda el archivo en el flujo proporcionado"
type: docs
weight: 70
url: /es/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Guarda el archivo en el flujo proporcionado.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outputStream | Flujo | Flujo de destino. |
| saveOptions | UueSaveOptions | Opciones para guardar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | No se ha proporcionado la fuente de datos a archivar. |
| ArgumentException | *outputStream* no es escribible. |
| UnauthorizedAccessException | La fuente del archivo es de solo lectura o es un directorio. |
| DirectoryNotFoundException | La ruta de la fuente de archivo especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | La fuente del archivo ya está abierta. |

## Observaciones

*outputStream* must be writable.

## Ejemplos

Escribir datos comprimidos al flujo de respuesta http.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Ver también

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Guarda el archivo en un archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| saveOptions | UueSaveOptions | Opciones para guardar el archivo. |

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
| InvalidOperationException | No se ha proporcionado la fuente de datos a archivar. |

## Ejemplos

Escribir datos codificados al archivo.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Ver también

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


