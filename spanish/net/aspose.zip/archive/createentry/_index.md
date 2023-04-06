---
title: Archive.CreateEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Archive método. Crear entrada única dentro del archivo.
type: docs
weight: 50
url: /es/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Crear entrada única dentro del archivo.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| path | String | El nombre completo del nuevo archivo o el nombre de archivo relativo que se comprimirá. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`ArchiveEntry`](../../archiveentry/) artículo. |

### Valor_devuelto

Instancia de entrada postal.

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

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*path* El parámetro no afecta el nombre de la entrada.

Si el archivo se abre inmediatamente con*openImmediately* parámetro se bloquea hasta que se guarda el archivo.

### Ejemplos

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Crear entrada única dentro del archivo.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| source | Stream | El flujo de entrada para la entrada. |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`ArchiveEntry`](../../archiveentry/) artículo. |

### Valor_devuelto

Instancia de entrada postal.

### Ejemplos

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Ver también

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Crear entrada única dentro del archivo.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo que se va a comprimir. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`ArchiveEntry`](../../archiveentry/) artículo. |

### Valor_devuelto

Instancia de entrada postal.

### Excepciones

| excepción | condición |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* es de solo lectura o es un directorio. |
| DirectoryNotFoundException | La ruta especificada no es válida, como estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*fileInfo* El parámetro no afecta el nombre de la entrada.

Si el archivo se abre inmediatamente con*openImmediately* parámetro se bloquea hasta que se guarda el archivo.

### Ejemplos

Componga un archivo con entradas encriptadas con diferentes métodos de encriptación y contraseñas cada una.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Ver también

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Crear entrada única dentro del archivo.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| source | Stream | El flujo de entrada para la entrada. |
| newEntrySettings | ArchiveEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`ArchiveEntry`](../../archiveentry/) artículo. |
| fileInfo | FileSystemInfo | Los metadatos del archivo o carpeta a comprimir. |

### Valor_devuelto

Instancia de entrada postal.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Ambos*source* y*fileInfo* son nulos o*source*es nulo y*fileInfo* significa directorio. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*fileInfo* El parámetro no afecta el nombre de la entrada.

*fileInfo* puede referirse aDirectoryInfo si la entrada es directorio.

### Ejemplos

Componer archivo con entrada cifrada.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Ver también

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)


