---
title: "Lz4Archive.SetSource"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método Lz4Archive. Establece el contenido que se comprimirá dentro del archivo."
type: docs
weight: 70
url: /es/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Flujo | El flujo de entrada para el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | El archivo está preparado para la extracción. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

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
| InvalidOperationException | El archivo está preparado para la extracción. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

Abra un archivo desde un flujo y extráigalo a un `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarArchive | TarArchive | Archivo Tar a comprimir. |
| formato | TarFormat | Define el formato de encabezado tar. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | Este archivo está preparado para la extracción. |

## Observaciones

Utilice este método para componer un archivo conjunto tar.lz4.

## Ejemplos

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Ver también

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | Ruta al archivo a comprimir. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| InvalidOperationException | Este archivo está preparado para la extracción. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

Abra un archivo desde la ruta del archivo y extráigalo a un `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


