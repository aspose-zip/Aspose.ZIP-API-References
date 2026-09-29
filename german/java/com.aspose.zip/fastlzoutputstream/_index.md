---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ein Stream-Wrapper, der Daten mit FastLZ komprimiert."
type: docs
weight: 68
url: /de/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Ein Stream-Wrapper, der Daten mit FastLZ komprimiert. Implementiert das Dekorateur-Muster.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Initialisiert eine neue Instanz der FastLZStream-Klasse, die für Kompression vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | Schließt den aktuellen Stream und gibt alle Ressourcen (wie Sockets und Dateihandles) frei, die mit dem aktuellen Stream verbunden sind. |
| [flush()](#flush--) | Leert alle Puffer für diesen Stream und veranlasst, dass alle gepufferten Daten auf das zugrunde liegende Gerät geschrieben werden. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Schreibt eine Sequenz von Bytes in den komprimierenden Stream und verschiebt die aktuelle Position innerhalb dieses Streams um die Anzahl der geschriebenen Bytes. |
| [write(int b)](#write-int-) | Schreibt das angegebene Byte in diesen Ausgabestream. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Initialisiert eine neue Instanz der FastLZStream-Klasse, die für Kompression vorbereitet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.OutputStream | der Stream zum Speichern komprimierter Daten |
| compressionLevel | int | Verwenden Sie 1 für schnellere Kompression, verwenden Sie 2 für ein besseres Kompressionsverhältnis. |

### close() {#close--}
```
public void close()
```


Schließt den aktuellen Stream und gibt alle Ressourcen (wie Sockets und Dateihandles) frei, die mit dem aktuellen Stream verbunden sind.

### flush() {#flush--}
```
public void flush()
```


Leert alle Puffer für diesen Stream und veranlasst, dass alle gepufferten Daten auf das zugrunde liegende Gerät geschrieben werden.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Schreibt eine Sequenz von Bytes in den komprimierenden Stream und verschiebt die aktuelle Position innerhalb dieses Streams um die Anzahl der geschriebenen Bytes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| buffer | byte[] | ein Array von Bytes. Diese Methode kopiert count Bytes vom Puffer in den aktuellen Stream. |
| offset | int | der nullbasierte Byte-Offset im Puffer, bei dem das Kopieren von Bytes in den aktuellen Stream beginnen soll |
| count | int | die Anzahl der Bytes, die in den aktuellen Stream geschrieben werden sollen |

### write(int b) {#write-int-}
```
public void write(int b)
```


Schreibt das angegebene Byte in diesen Ausgabestream. Der allgemeine Vertrag für `write` ist, dass ein Byte in den Ausgabestream geschrieben wird. Das zu schreibende Byte sind die acht niederwertigen Bits des Arguments `b`. Die 24 höherwertigen Bits von `b` werden ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| b | int | das `byte` |

