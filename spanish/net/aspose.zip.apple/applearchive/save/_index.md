---
title: "AppleArchive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método AppleArchive. Guarda el archivo en el flujo proporcionado."
type: docs
weight: 90
url: /es/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Guarda el archivo en el flujo proporcionado.

```csharp
public void Save(Stream output)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| salida | Flujo | Flujo de destino. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado. |
| ArgumentNullException | *output* es `null`. |
| ArgumentException | *output* no es escribible. |
| ArgumentOutOfRangeException | El tamaño de bloque configurado para LZ4 o Zlib no es positivo. |
| NotSupportedException | Faltan los ajustes de compresión o no son compatibles, la composición directa utiliza un flujo no buscable, o el tamaño de la entrada/archivo supera los límites actuales de Apple Archive. |

## Observaciones

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Ver también

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Guarda el archivo en un archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se creará. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado. |
| ArgumentException | *destinationFileName* es inválido. |
| ArgumentNullException | *destinationFileName* es `null`. |
| ArgumentOutOfRangeException | El tamaño de bloque configurado para LZ4 o Zlib no es positivo. |
| NotSupportedException | Faltan los ajustes de compresión o no son compatibles, la composición directa utiliza un flujo no buscable, o el tamaño de la entrada/archivo supera los límites actuales de Apple Archive. |

### Ver también

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


