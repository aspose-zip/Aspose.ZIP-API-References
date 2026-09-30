---
title: "UueArchive.SetSource"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método UueArchive. Establece el contenido que se codificará dentro del archivo"
type: docs
weight: 80
url: /es/net/aspose.zip.uue/uuearchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Establece el contenido que se codificará dentro del archivo.

```csharp
public void SetSource(Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Flujo | El flujo de entrada para el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.uue");
}
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | La referencia a un archivo que será comprimido. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.uue");
}
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Establece el contenido que se codificará dentro del archivo.

```csharp
public void SetSource(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | Ruta al archivo que será codificado. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |

## Ejemplos

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


