---
title: CpioEntry.Extract
second_title: Referencia de la API de Aspose.ZIP para .NET
description: CpioEntry método. Extrae la entrada al sistema de archivos por la ruta proporcionada.
type: docs
weight: 60
url: /es/net/aspose.zip.cpio/cpioentry/extract/
---
## Extract(string) {#extract}

Extrae la entrada al sistema de archivos por la ruta proporcionada.

```csharp
public FileSystemInfo Extract(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta al archivo de destino. Si el archivo ya existe, se sobrescribirá. |

### Valor_devuelto

La información del archivo del archivo compuesto.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Ejemplos

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Ver también

* class [CpioEntry](../)
* espacio de nombres [Aspose.Zip.Cpio](../../cpioentry/)
* asamblea [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrae la entrada al flujo proporcionado.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destination | Stream | Flujo de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destination* no admite la escritura. |

### Ejemplos

Extraiga una entrada del archivo cpio.

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Ver también

* class [CpioEntry](../)
* espacio de nombres [Aspose.Zip.Cpio](../../cpioentry/)
* asamblea [Aspose.Zip](../../../)


