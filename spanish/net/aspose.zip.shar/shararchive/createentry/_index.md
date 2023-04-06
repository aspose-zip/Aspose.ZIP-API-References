---
title: SharArchive.CreateEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SharArchive método. Crear entrada única dentro del archivo.
type: docs
weight: 40
url: /es/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Crear entrada única dentro del archivo.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo o carpeta a comprimir. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |

### Valor_devuelto

Instancia de entrada compartida.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *name* es nulo. |
| ArgumentException | *name* esta vacio. |
| ArgumentNullException | *fileInfo* es nulo. |

### Observaciones

Si el archivo se abre inmediatamente con*openImmediately*parámetro se bloquea hasta que se elimine el archivo.

### Ejemplos

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Ver también

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Crear entrada única dentro del archivo.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| sourcePath | String | Ruta al archivo a comprimir. |
| openImmediately | Boolean | Verdadero si abre el archivo inmediatamente; de lo contrario, abra el archivo al guardar el archivo. |

### Valor_devuelto

Instancia de entrada compartida.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourcePath* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*sourcePath* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. - o - Nombre de archivo, como parte de*name*, supera los 100 símbolos. |
| UnauthorizedAccessException | Acceso al archivo*sourcePath* es denegado. |
| PathTooLongException | El especificado*sourcePath* , nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. - o -*name* es demasiado largo para shar. |
| NotSupportedException | Archivo en*sourcePath* contiene dos puntos (:) en medio de la cadena. |

### Observaciones

El nombre de la entrada se establece únicamente dentro*name* parámetro. El nombre del archivo proporcionado en*sourcePath* El parámetro no afecta el nombre de la entrada.

Si el archivo se abre inmediatamente con*openImmediately*parámetro se bloquea hasta que se elimine el archivo.

### Ejemplos

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Ver también

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Crear entrada única dentro del archivo.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| source | Stream | El flujo de entrada para la entrada. |

### Valor_devuelto

Instancia de entrada compartida.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *name* es nulo. |
| ArgumentNullException | *source* es nulo. |
| ArgumentException | *name* esta vacio. |

### Ejemplos

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Ver también

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)


