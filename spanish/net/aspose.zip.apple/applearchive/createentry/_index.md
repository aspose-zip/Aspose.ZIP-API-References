---
title: "AppleArchive.CreateEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método AppleArchive. Crea una única entrada dentro del archivo"
type: docs
weight: 60
url: /es/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Crea una única entrada dentro del archivo.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| ruta | String | La ruta al archivo a comprimir. |
| openImmediately | Boolean | True, si se abre el archivo inmediatamente, de lo contrario se abre al guardar el archivo. |

### Valor devuelto

Instancia de entrada de Apple Archive.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado. |
| ArgumentException | *name* está vacío. |
| ArgumentNullException | *path* es `null`. |

### Ver también

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Crea una única entrada dentro del archivo.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| origen | Flujo | El flujo de entrada para la entrada. |

### Valor devuelto

Instancia de entrada de Apple Archive.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado. |
| ArgumentException | *name* está vacío. |
| ArgumentNullException | *source* es `null`. |

### Ver también

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Crea una única entrada dentro del archivo.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la entrada. |
| fileInfo | FileInfo | Los metadatos del archivo a comprimir. |
| openImmediately | Boolean | True, si se abre el archivo inmediatamente, de lo contrario se abre al guardar el archivo. |

### Valor devuelto

Instancia de entrada de Apple Archive.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado. |
| ArgumentException | *name* está vacío. |
| ArgumentNullException | *fileInfo* es `null`. |

### Ver también

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


