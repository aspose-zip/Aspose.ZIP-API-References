---
title: SetSource
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Establece el contenido que se comprimirá dentro del archivo.
type: docs
weight: 60
url: /es/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | El flujo de entrada para el archivo. |

### Ejemplos

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### Ver también

* class [Bzip2Archive](../../bzip2archive)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | La referencia a un archivo que se va a comprimir. |

### Ejemplos

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### Ver también

* class [Bzip2Archive](../../bzip2archive)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

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
| SecurityException | La persona que llama no tiene el permiso requerido para acceder |
| ArgumentException | los*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Ejemplos

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Ver también

* class [Bzip2Archive](../../bzip2archive)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| tarArchive | TarArchive | Tar archivo para ser comprimido. |
| format | TarFormat | Define el formato del encabezado tar. |

### Observaciones

Utilice este método para crear un archivo conjunto tar.bz2.

### Ejemplos

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### Ver también

* class [TarArchive](../../../aspose.zip.tar/tararchive)
* enum [TarFormat](../../../aspose.zip.tar/tarformat)
* class [Bzip2Archive](../../bzip2archive)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive)
* asamblea [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Establece el contenido que se comprimirá dentro del archivo.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| cpioArchive | CpioArchive | Archivo Cpio a comprimir. |
| format | CpioFormat | Define el formato del encabezado cpio. |

### Observaciones

Utilice este método para crear un archivo cpio.bz2 conjunto.

### Ejemplos

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### Ver también

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat)
* class [Bzip2Archive](../../bzip2archive)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive)
* asamblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
