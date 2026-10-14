---
title: "CabArchive.CreateEntries"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método CabArchive. Agrega al archivo todos los archivos recursivamente desde el directorio especificado"
type: docs
weight: 30
url: /es/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Agrega al archivo todos los archivos, recursivamente, desde el directorio especificado.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | DirectoryInfo | Directorio a comprimir. |
| includeRootDirectory | Boolean | Indica si se debe incluir el nombre del directorio raíz en las rutas de las entradas. |

### Valor devuelto

La instancia actual de [`CabArchive`](../).

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *directory* es nulo. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| DirectoryNotFoundException | *directory* no se puede encontrar. |
| SecurityException | El llamador no tiene el permiso requerido para acceder a *directory* o a su contenido. |
| UnauthorizedAccessException | El acceso a *directory* o a uno de sus archivos está denegado. |
| IOException | Se produce un error de E/S al acceder a *directory*. |
| PathTooLongException | Una ruta de entrada generada supera la longitud máxima definida por el sistema. |
| InvalidOperationException | El archivo está preparado para extracción y no puede agregar entradas. |

## Ejemplos

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Ver también

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Agrega al archivo todos los archivos de forma recursiva desde la ruta de directorio especificada.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | String | Ruta del directorio a comprimir. |
| includeRootDirectory | Boolean | Indica si se debe incluir el nombre del directorio raíz en las rutas de las entradas. |

### Valor devuelto

La instancia actual de [`CabArchive`](../).

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | *sourceDirectory* es nulo. |
| DirectoryNotFoundException | *sourceDirectory* no se puede encontrar. |
| SecurityException | El llamador no tiene el permiso requerido para acceder a *sourceDirectory*. |
| UnauthorizedAccessException | El acceso a *sourceDirectory* está denegado. |
| PathTooLongException | El *sourceDirectory* especificado supera la longitud máxima definida por el sistema. |
| ArgumentException | *sourceDirectory* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. |
| IOException | Se produce un error de E/S al acceder a *sourceDirectory*. |
| InvalidOperationException | El archivo está preparado para extracción y no puede agregar entradas. |

## Ejemplos

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Ver también

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


