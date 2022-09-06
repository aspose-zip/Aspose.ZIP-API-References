---
title: CreateEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Crear entrada única dentro del archivo.
type: docs
weight: 80
url: /es/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Crear entrada única dentro del archivo.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| source | Stream | El flujo de entrada para la entrada. |
| fileInfo | FileSystemInfo | Los metadatos del archivo o carpeta a comprimir. |

### Valor_devuelto

Instancia de entrada de alquitrán.

### Excepciones

| excepción | condición |
| --- | --- |
| PathTooLongException | *name* es demasiado largo para tar según el estándar IEEE 1003.1-1998. |
| ArgumentException | Nombre de archivo, como parte de*name*, supera los 100 símbolos. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*fileInfo* El parámetro no afecta el nombre de la entrada.

*fileInfo* puede referirse aDirectoryInfo si la entrada es directorio.

### Ejemplos

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Ver también

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Crear entrada única dentro del archivo.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo o carpeta a comprimir. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |

### Valor_devuelto

Instancia de entrada de alquitrán.

### Excepciones

| excepción | condición |
| --- | --- |
| PathTooLongException | *name* es demasiado largo para tar según el estándar IEEE 1003.1-1998. |
| ArgumentException | Nombre de archivo, como parte de*name*, supera los 100 símbolos. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*fileInfo* El parámetro no afecta el nombre de la entrada.

*fileInfo* puede referirse aDirectoryInfo si la entrada es directorio.

Si el archivo se abre inmediatamente con*openImmediately* parámetro se bloquea hasta que se elimine el archivo.

### Ejemplos

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Ver también

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Crear entrada única dentro del archivo.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| path | String | Ruta al archivo a comprimir. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |

### Valor_devuelto

Instancia de entrada de alquitrán.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso requerido para acceder |
| ArgumentException | los*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. - o - Nombre de archivo, como parte de*name*, supera los 100 símbolos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path* , nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. - o -*name* es demasiado largo para tar según el estándar IEEE 1003.1-1998. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*path* El parámetro no afecta el nombre de la entrada.

Si el archivo se abre inmediatamente con*openImmediately* parámetro se bloquea hasta que se elimine el archivo.

### Ejemplos

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Ver también

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive)
* asamblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
