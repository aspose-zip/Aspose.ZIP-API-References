---
title: "ZstandardArchive.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método ZstandardArchive. Extrae el archivo al flujo proporcionado"
type: docs
weight: 30
url: /es/net/aspose.zip.zstandard/zstandardarchive/extract/
---
## Extract(Stream) {#extract_1}

Extrae el archivo al flujo proporcionado.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | Flujo | Secuencia de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentException | *destination* no admite escritura. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |

## Ejemplos

```csharp
using (var archive = new GzipArchive("archive.zst"))
{
     archive.Extract(httpResponseStream);
}
```

### Ver también

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrae el archivo al archivo por ruta.

```csharp
public FileInfo Extract(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

### Valor devuelto

Información de un archivo extraído.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |

### Ver también

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


