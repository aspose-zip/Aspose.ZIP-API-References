---
title: "FastLZOutputStream"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Un contenedor de flujo que comprime datos con FastLZ."
type: docs
weight: 68
url: /es/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Un contenedor de flujo que comprime datos con FastLZ. Implementa el patrón decorador.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Inicializa una nueva instancia de la clase FastLZStream preparada para compresión. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | Cierra el flujo actual y libera cualquier recurso (como sockets y manejadores de archivos) asociado al flujo actual. |
| [flush()](#flush--) | Limpia todos los búferes de este flujo y hace que cualquier dato almacenado en búfer se escriba en el dispositivo subyacente. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Escribe una secuencia de bytes en el flujo de compresión y avanza la posición actual dentro de este flujo en la cantidad de bytes escritos. |
| [write(int b)](#write-int-) | Escribe el byte especificado en este flujo de salida. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Inicializa una nueva instancia de la clase FastLZStream preparada para compresión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | el flujo para guardar datos comprimidos |
| compressionLevel | int | use 1 para una compresión más rápida, use 2 para una mejor relación de compresión |

### close() {#close--}
```
public void close()
```


Cierra el flujo actual y libera cualquier recurso (como sockets y manejadores de archivos) asociado al flujo actual.

### flush() {#flush--}
```
public void flush()
```


Limpia todos los búferes de este flujo y hace que cualquier dato almacenado en búfer se escriba en el dispositivo subyacente.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Escribe una secuencia de bytes en el flujo de compresión y avanza la posición actual dentro de este flujo en la cantidad de bytes escritos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| buffer | byte[] | una matriz de bytes. Este método copia count bytes desde buffer al flujo actual |
| offset | int | el desplazamiento de byte basado en cero en buffer en el que comenzar a copiar bytes al flujo actual |
| count | int | el número de bytes que se escribirán en el flujo actual |

### write(int b) {#write-int-}
```
public void write(int b)
```


Escribe el byte especificado en este flujo de salida. El contrato general para `write` es que se escribe un byte en el flujo de salida. El byte a escribir son los ocho bits de menor orden del argumento `b`. Los 24 bits de mayor orden de `b` se ignoran.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| b | int | el `byte` |

