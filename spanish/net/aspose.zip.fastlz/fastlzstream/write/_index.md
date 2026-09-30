---
title: "FastLZStream.Write"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método FastLZStream. Escribe una secuencia de bytes en el flujo de compresión y avanza la posición actual dentro de este flujo en la cantidad de bytes escritos"
type: docs
weight: 120
url: /es/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Escribe una secuencia de bytes en el flujo de compresión y avanza la posición actual dentro de este flujo por la cantidad de bytes escritos.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| búfer | Byte[] | Una matriz de bytes. Este método copia count bytes desde buffer al flujo actual. |
| desplazamiento | Int32 | El desplazamiento de bytes basado en cero en buffer desde el cual comenzar a copiar bytes al flujo actual. |
| count | Int32 | El número de bytes que se escribirán en el flujo actual. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | Lanzada si el flujo ha sido descartado. |
| ArgumentNullException | *buffer* es `null`. |

### Ver también

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


