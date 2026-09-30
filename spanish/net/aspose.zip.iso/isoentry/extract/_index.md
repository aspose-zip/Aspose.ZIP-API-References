---
title: "IsoEntry.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método IsoEntry. Extrae la entrada al sistema de archivos mediante la ruta proporcionada"
type: docs
weight: 50
url: /es/net/aspose.zip.iso/isoentry/extract/
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

Instancia de FileInfo que contiene los datos extraídos.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| FileNotFoundException | El archivo no se encuentra. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| InvalidOperationException | No se leyeron los encabezados del archivo y la información del servicio. |

### Ver también

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| NotSupportedException | Se lanza si la entrada no representa un archivo. |
| ArgumentException | La secuencia proporcionada no admite escritura. |

### Ver también

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


