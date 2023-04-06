---
title: XarArchive.XarArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: XarArchive constructor. Inicializa una nueva instancia delXarArchive La lista de entradas de clases y composiciones se puede extraer del archivo.
type: docs
weight: 10
url: /es/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Inicializa una nueva instancia del[`XarArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public XarArchive(Stream sourceStream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceStream | Stream | La fuente del archivo. Debe ser buscable. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceStream* es nulo. |
| ArgumentException | *sourceStream* no es buscable. |
| InvalidDataException | *sourceStream* no es un archivo xar válido. |

### Observaciones

Este constructor no desempaqueta ninguna entrada. Ver[`Open`](../../xarfileentry/open/)método para desempaquetar.

### Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [XarArchive](../)
* espacio de nombres [Aspose.Zip.Xar](../../xararchive/)
* asamblea [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Inicializa una nueva instancia del[`XarArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public XarArchive(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta al archivo de almacenamiento. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Observaciones

Este constructor no desempaqueta ninguna entrada. Ver[`Open`](../../xarfileentry/open/)método para desempaquetar.

### Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [XarArchive](../)
* espacio de nombres [Aspose.Zip.Xar](../../xararchive/)
* asamblea [Aspose.Zip](../../../)


