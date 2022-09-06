---
title: Archive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Inicializa una nueva instancia delArchiveaspose.zip/archiveclase con configuraciones opcionales para sus entradas.
type: docs
weight: 10
url: /es/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Inicializa una nueva instancia del[`Archive`](../../archive)clase con configuraciones opcionales para sus entradas.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para recién agregados[`ArchiveEntry`](../../archiveentry)items. Si no se especifica, se usará la compresión Deflate sin cifrado más común. |

### Ejemplos

El siguiente ejemplo muestra cómo comprimir un solo archivo con la configuración predeterminada.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Ver también

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* espacio de nombres [Aspose.Zip](../../archive)
* asamblea [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Inicializa una nueva instancia del[`Archive`](../../archive) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceStream | Stream | La fuente del archivo. |
| loadOptions | ArchiveLoadOptions | Opciones para cargar el archivo existente. |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para recién agregados[`ArchiveEntry`](../../archiveentry)items. Si no se especifica, se usará la compresión Deflate sin cifrado más común. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *sourceStream* no es buscable. |
| InvalidDataException | El encabezado de cifrado para AES contradice el método de compresión de WinZip. |

### Observaciones

Este constructor no descomprime ninguna entrada. Ver[`Open`](../../archiveentry/open) método para descomprimir.

### Ejemplos

El siguiente ejemplo extrae un archivo cifrado, luego descomprime la primera entrada a un`Flujo de memoria`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ver también

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* espacio de nombres [Aspose.Zip](../../archive)
* asamblea [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Inicializa una nueva instancia del[`Archive`](../../archive) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta completa o relativa al archivo de almacenamiento. |
| loadOptions | ArchiveLoadOptions | Opciones para cargar el archivo existente. |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para recién agregados[`ArchiveEntry`](../../archiveentry)items. Si no se especifica, se usará la compresión Deflate sin cifrado más común. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso requerido para acceder |
| ArgumentException | los*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Observaciones

Este constructor no descomprime ninguna entrada. Ver[`Open`](../../archiveentry/open) método para descomprimir.

### Ejemplos

El siguiente ejemplo extrae un archivo cifrado, luego descomprime la primera entrada a un`Flujo de memoria`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ver también

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* espacio de nombres [Aspose.Zip](../../archive)
* asamblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
