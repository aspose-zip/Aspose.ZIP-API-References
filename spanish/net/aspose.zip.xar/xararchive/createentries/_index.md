---
title: "XarArchive.CreateEntries"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método XarArchive. Añade al archivo todos los archivos y directorios de forma recursiva en el directorio especificado"
type: docs
weight: 30
url: /es/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Añade al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | String | Directorio a comprimir. |
| compressionSettings | Boolean | La configuración de compresión utilizada para los elementos [`XarEntry`](../../xarentry/) añadidos. |
| includeRootDirectory | XarCompressionSettings | Indica si se debe incluir el directorio raíz mismo o no. |

### Valor devuelto

Instancia de entrada Xar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceDirectory* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder a *sourceDirectory*. |
| ArgumentException | *sourceDirectory* contiene caracteres no válidos como ", &lt;, &gt;, o &#x7C;.; |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. La ruta especificada, el nombre de archivo, o ambos son demasiado largos. |
| IOException | *sourceDirectory* representa un archivo, no un directorio. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Ver también

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Añade al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | DirectoryInfo | Directorio a comprimir. |
| compressionSettings | Boolean | La configuración de compresión utilizada para los elementos [`XarEntry`](../../xarentry/) añadidos. |
| includeRootDirectory | XarCompressionSettings | Indica si se debe incluir el directorio raíz mismo o no. |

### Valor devuelto

Instancia de entrada Xar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *directory* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder a *directory*. |
| IOException | *directory* representa un archivo, no un directorio. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Ver también

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


