---
title: "XarArchive.CreateEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "XarArchive método. Crea una única entrada dentro del archivo"
type: docs
weight: 40
url: /es/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Crea una única entrada dentro del archivo.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo o carpeta a comprimir. |
| openImmediately | Boolean | True, si se abre el archivo inmediatamente, de lo contrario se abre al guardar el archivo. |
| compressionSettings | XarCompressionSettings | La configuración de compresión utilizada para el elemento [`XarEntry`](../../xarentry/) añadido. |

### Valor devuelto

Instancia de entrada Xar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *name* es nulo. |
| ArgumentException | *name* está vacío. |
| ArgumentNullException | *fileInfo* es nulo. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

Si el archivo se abre inmediatamente con el parámetro *openImmediately* queda bloqueado hasta que el archivo se libere.

## Ejemplos

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Ver también

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Crea una única entrada dentro del archivo.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| sourcePath | String | Ruta al archivo a comprimir. |
| openImmediately | Boolean | True, si se abre el archivo inmediatamente, de lo contrario se abre al guardar el archivo. |
| compressionSettings | XarCompressionSettings | La configuración de compresión utilizada para el elemento [`XarEntry`](../../xarentry/) añadido. |

### Valor devuelto

Instancia de entrada Xar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourcePath* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | El *sourcePath* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. - or - El nombre de archivo, como parte de *name*, supera los 100 símbolos. |
| UnauthorizedAccessException | Acceso al archivo *sourcePath* denegado. |
| PathTooLongException | El *sourcePath* especificado, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. - or - *name* es demasiado largo para xar. |
| NotSupportedException | El archivo en *sourcePath* contiene dos puntos (:) en medio de la cadena. |
| InvalidOperationException | Imposible modificar el archivo xar. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

El nombre de la entrada se establece únicamente dentro del parámetro *name*. El nombre de archivo proporcionado en el parámetro *sourcePath* no afecta al nombre de la entrada.

Si el archivo se abre inmediatamente con el parámetro *openImmediately* queda bloqueado hasta que el archivo se libere.

## Ejemplos

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Ver también

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Crea una única entrada dentro del archivo.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| origen | Flujo | El flujo de entrada para la entrada. |
| compressionSettings | XarCompressionSettings | La configuración de compresión utilizada para el elemento [`XarEntry`](../../xarentry/) añadido. |

### Valor devuelto

Instancia de entrada Xar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *name* es nulo. |
| ArgumentNullException | *source* es nulo. |
| ArgumentException | *name* está vacío. |
| InvalidOperationException | Imposible modificar el archivo xar. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Ver también

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


