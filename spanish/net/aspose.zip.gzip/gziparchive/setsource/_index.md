---
title: GzipArchive.SetSource
second_title: Referencia de la API de Aspose.ZIP para .NET
description: GzipArchive método. Establece el contenido que se comprimirá dentro del archivo.
type: docs
weight: 70
url: /es/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | El flujo de entrada para el archivo. |

### Ejemplos

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Ver también

* class [GzipArchive](../)
* espacio de nombres [Aspose.Zip.Gzip](../../gziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | La referencia a un archivo que se va a comprimir. |

### Ejemplos

Abra un archivo de una secuencia y extráigalo a un`Flujo de memoria`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Ver también

* class [GzipArchive](../)
* espacio de nombres [Aspose.Zip.Gzip](../../gziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | Ruta al archivo a comprimir. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Ejemplos

Abra un archivo de archivo por ruta y extráigalo a un`Flujo de memoria`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Ver también

* class [GzipArchive](../)
* espacio de nombres [Aspose.Zip.Gzip](../../gziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| tarArchive | TarArchive | Tar archivo para ser comprimido. |

### Observaciones

Utilice este método para crear un archivo tar.gz conjunto.

### Ejemplos

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Ver también

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* espacio de nombres [Aspose.Zip.Gzip](../../gziparchive/)
* asamblea [Aspose.Zip](../../../)


