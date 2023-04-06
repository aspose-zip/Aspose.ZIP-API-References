---
title: SevenZipArchive.CreateEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipArchive método. Crear entrada única dentro del archivo.
type: docs
weight: 50
url: /es/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Crear entrada única dentro del archivo.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo que se va a comprimir. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |
| newEntrySettings | SevenZipEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) artículo. |

### Valor_devuelto

Instancia de siete entradas Zip.

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

Componga un archivo con entradas cifradas con diferentes contraseñas cada una.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Ver también

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Crear entrada única dentro del archivo.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| source | Stream | El flujo de entrada para la entrada. |
| newEntrySettings | SevenZipEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) artículo. |
| fileInfo | FileSystemInfo | Los metadatos del archivo o carpeta a comprimir. |

### Valor_devuelto

Instancia de entrada de SevenZip.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Ambos*source* y*fileInfo* son nulos o*source*es nulo y*fileInfo* significa directorio. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*fileInfo* El parámetro no afecta el nombre de la entrada.

*fileInfo* puede referirse aDirectoryInfo si la entrada es directorio.

### Ejemplos

Componer archivo con entrada cifrada comprimida LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Ver también

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Crear entrada única dentro del archivo.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| source | Stream | El flujo de entrada para la entrada. |
| newEntrySettings | SevenZipEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) artículo. |

### Valor_devuelto

Instancia de entrada postal.

### Ejemplos

Componga un archivo 7z con compresión LZMA2 y encriptación de todas las entradas.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Ver también

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Crear entrada única dentro del archivo.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| path | String | El nombre completo del nuevo archivo o el nombre de archivo relativo que se comprimirá. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |
| newEntrySettings | SevenZipEntrySettings | Configuraciones de compresión y encriptación usadas para agregar[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) artículo. |

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
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Ver también

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)


