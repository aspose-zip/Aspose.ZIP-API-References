---
title: "AlzEntry.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método AlzEntry. Extrae la entrada al sistema de archivos usando la ruta proporcionada"
type: docs
weight: 60
url: /es/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |
| contraseña | String | Contraseña opcional para descifrado. |

### Valor devuelto

La información del archivo de un archivo compuesto.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| InvalidDataException | El archivo está corrupto. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| FileNotFoundException | El archivo no se encuentra. |

## Ejemplos

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Ver también

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extrae la entrada al flujo proporcionado.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | Flujo | Secuencia de destino. Debe ser escribible. |
| contraseña | String | Contraseña opcional para descifrado. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destination* no admite escritura. |
| InvalidOperationException | El archivo no está abierto para extracción. - o - Esta entrada es un directorio. |
| InvalidDataException | Datos incorrectos dentro de la entrada. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |

## Ejemplos

Extraer una entrada del archivo ALZ con contraseña.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Ver también

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


