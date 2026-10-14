---
title: "Lz4Archive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método Lz4Archive. Guarda el archivo lz4 en el flujo proporcionado"
type: docs
weight: 60
url: /es/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Guarda el archivo lz4 en el flujo proporcionado.

```csharp
public void Save(Stream output)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| salida | Flujo | Flujo de destino. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *output* es nulo. |
| ArgumentException | *output* no es escribible. |
| InvalidOperationException | El archivo está preparado para la extracción. - o - No se proporcionó la fuente. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Lanzada cuando la compresión se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

*output* must be seekable.

## Ejemplos

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Guarda el archivo lz4 en el archivo de destino proporcionado.

```csharp
public void Save(FileInfo destination)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | FileInfo | FileInfo, que se abrirá como flujo de destino. |

### Excepciones

| excepción | condición |
| --- | --- |
| SecurityException | El llamador no tiene el permiso requerido para abrir el *destino*. |
| ArgumentException | La ruta del archivo está vacía o contiene solo espacios en blanco. |
| FileNotFoundException | El archivo no se encuentra. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *destino* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| InvalidOperationException | El archivo está preparado para la extracción. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destinationFileName* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder |
| ArgumentException | El *destinationFileName* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *destinationFileName* denegado. |
| PathTooLongException | El *destinationFileName* especificado, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *destinationFileName* contiene dos puntos (:) en medio de la cadena. |
| InvalidOperationException | El archivo está preparado para la extracción. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| DirectoryNotFoundException | La ruta especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| FileNotFoundException | No se encontró el archivo especificado en *destinationFileName*. |
| IOException | Se produjo un error de E/S al abrir el archivo. |

## Ejemplos

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


