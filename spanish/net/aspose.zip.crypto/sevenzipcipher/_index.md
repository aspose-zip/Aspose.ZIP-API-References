---
title: Class SevenZipCipher
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Crypto.SevenZipCipher clase. Clase base para el cifrado AES utilizado para el cifrado 7zip.
type: docs
weight: 190
url: /es/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Clase base para el cifrado AES utilizado para el cifrado 7-zip.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Obtiene un valor que indica si la transformación actual se puede reutilizar. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Obtiene un valor que indica si se pueden transformar varios bloques. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Obtiene el tamaño del bloque de entrada. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Obtiene el tamaño del bloque de salida. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Transforma la región especificada de la matriz de bytes de entrada y copia la transformación resultante en la región especificada de la matriz de bytes de salida. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Transforma la región especificada de la matriz de bytes especificada. |

### Ver también

* espacio de nombres [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* asamblea [Aspose.Zip](../../)


