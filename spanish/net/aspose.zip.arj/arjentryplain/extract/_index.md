---
title: "ArjEntryPlain.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método ArjEntryPlain. Extrae la entrada al sistema de archivos mediante la ruta proporcionada"
type: docs
weight: 40
url: /es/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

```csharp
public FileInfo Extract(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

### Valor devuelto

La información del archivo de un archivo compuesto.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo o está vacío. |
| ObjectDisposedException | Se lanza si el archivo ha sido descartado. |
| FileNotFoundException | El archivo no se encuentra. |
| InvalidDataException | Desajuste de suma de verificación para encabezados o datos. - o - El archivo está corrupto. |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. |
| NotImplementedException | Entrada comprimida con el método 4. |

## Ejemplos

Extrae dos entradas del archivo rar.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Ver también

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrae la entrada del archivo ARJ a un archivo.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo para almacenar datos descomprimidos. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | No se leyeron los encabezados del archivo y la información del servicio. |
| SecurityException | El llamador no tiene el permiso requerido para abrir el *fileInfo*. |
| ArgumentException | La ruta del archivo está vacía o contiene solo espacios en blanco. |
| FileNotFoundException | El archivo no se encuentra. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *fileInfo* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el archivo ha sido descartado. |
| InvalidDataException | Desajuste de suma de verificación para encabezados o datos. - o - El archivo está corrupto. |
| NotImplementedException | Entrada comprimida con el método 4. |

## Ejemplos

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ver también

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Extrae la entrada al flujo proporcionado.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | Flujo | Secuencia de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destination* no admite escritura. |
| InvalidDataException | Desajuste de suma de verificación para encabezados o datos. - o - El archivo está corrupto. |
| NotImplementedException | Entrada comprimida con el método 4. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el archivo ha sido descartado. |

### Ver también

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


