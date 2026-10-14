---
title: "AppleArchive.AppleArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "AppleArchive constructor. Inicializa una nueva instancia de la clase AppleArchive con la configuración utilizada para entradas compuestas."
type: docs
weight: 10
url: /es/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Inicializa una nueva instancia de la clase [`AppleArchive`](../) con la configuración utilizada para entradas compuestas.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Configuración utilizada al componer un nuevo Apple Archive. |

### Ver también

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`AppleArchive`](../) y compone una lista de entradas que puede extraerse del archivo.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | Flujo | La fuente del archivo. |
| loadOptions | AppleArchiveLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceStream* es nulo. |
| ArgumentException | *sourceStream* no es desplazable. |
| InvalidDataException | *sourceStream* no es un Apple Archive válido. |
| EndOfStreamException | El flujo termina inesperadamente durante el análisis de las entradas del archivo. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte los métodos [`ExtractToDirectory`](../extracttodirectory/) y [`Open`](../../applearchiveentry/open/) para descomprimir.

### Ver también

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Inicializa una nueva instancia de la clase [`AppleArchive`](../) y compone una lista de entradas que puede extraerse del archivo.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta completa o relativa al archivo del archivo. |
| loadOptions | AppleArchiveLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| FileNotFoundException | El archivo no se encuentra. |
| InvalidDataException | *path* no es un Apple Archive válido. |
| EndOfStreamException | El flujo termina inesperadamente durante el análisis de las entradas del archivo. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte los métodos [`ExtractToDirectory`](../extracttodirectory/) y [`Open`](../../applearchiveentry/open/) para descomprimir.

### Ver también

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


