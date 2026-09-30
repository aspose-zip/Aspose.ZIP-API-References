---
title: "CabArchive.CreateEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método CabArchive. Crea una única entrada dentro del archivo"
type: docs
weight: 40
url: /es/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Crea una única entrada dentro del archivo.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| ruta | String | El nombre totalmente calificado del nuevo archivo, o el nombre de archivo relativo que se comprimirá. |
| newEntrySettings | CabEntrySettings | Configuración de compresión y cifrado utilizada para el elemento [`CabEntry`](../../cabentry/) añadido. |

### Valor devuelto

Instancia de entrada Cab.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | El archivo está preparado para extracción y no puede agregar entradas. |

## Observaciones

El nombre de la entrada se establece únicamente dentro del parámetro *name*. El nombre de archivo proporcionado en el parámetro *path* no afecta al nombre de la entrada.

## Ejemplos

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Ver también

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Crea una única entrada dentro del archivo.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| origen | Flujo | El flujo de entrada para la entrada. |
| newEntrySettings | CabEntrySettings | Configuración de compresión y cifrado utilizada para el elemento [`CabEntry`](../../cabentry/) añadido. |

### Valor devuelto

Instancia de entrada Cab.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | El archivo está preparado para extracción y no puede agregar entradas. |
| ArgumentNullException | *name* es nulo. |

## Ejemplos

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Ver también

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Crea una única entrada dentro del archivo.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo a comprimir. |
| newEntrySettings | CabEntrySettings | Configuración de compresión y cifrado utilizada para el elemento [`CabEntry`](../../cabentry/) añadido. |

### Valor devuelto

Instancia de entrada CAB.

### Excepciones

| excepción | condición |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* es de solo lectura o es un directorio. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| FileNotFoundException | *fileInfo* representa un archivo que no se puede encontrar. |
| SecurityException | El llamador no tiene el permiso requerido para acceder a *fileInfo*. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | El archivo está preparado para extracción y no puede agregar entradas. |
| ArgumentNullException | *name* es nulo. |

## Observaciones

El nombre de la entrada se establece únicamente dentro del parámetro *name*. El nombre de archivo proporcionado en el parámetro *fileInfo* no afecta al nombre de la entrada.

## Ejemplos

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Ver también

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Crea una única entrada dentro del archivo.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| streamProvider | Func`1 | El método que proporciona el flujo de entrada para la entrada. |
| newEntrySettings | CabEntrySettings | Configuración de compresión y cifrado utilizada para el elemento [`CabEntry`](../../cabentry/) añadido. |

### Valor devuelto

Instancia de entrada CAB.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | El archivo se instancia para descompresión. - o - El número de archivos ha alcanzado el límite. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentException | El *name* es nulo o está vacío. |

## Ejemplos

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Ver también

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


