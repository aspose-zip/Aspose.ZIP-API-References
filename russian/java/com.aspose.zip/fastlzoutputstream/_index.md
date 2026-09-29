---
title: "FastLZOutputStream"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Обёртка потока, сжимающая данные с помощью FastLZ."
type: docs
weight: 68
url: /ru/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Обёртка потока, которая сжимает данные с помощью FastLZ. Реализует шаблон декоратора.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Инициализирует новый экземпляр класса FastLZStream, подготовленный для сжатия. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | Закрывает текущий поток и освобождает любые ресурсы (например, сокеты и файловые дескрипторы), связанные с текущим потоком. |
| [flush()](#flush--) | Очищает все буферы этого потока и заставляет любые буферизованные данные записаться в нижележащее устройство. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Записывает последовательность байтов в сжимающий поток и перемещает текущую позицию в этом потоке на количество записанных байтов. |
| [write(int b)](#write-int-) | Записывает указанный байт в этот выходной поток. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Инициализирует новый экземпляр класса FastLZStream, подготовленный для сжатия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | поток для сохранения сжатых данных |
| compressionLevel | int | используйте 1 для более быстрого сжатия, используйте 2 для лучшего коэффициента сжатия |

### close() {#close--}
```
public void close()
```


Закрывает текущий поток и освобождает любые ресурсы (например, сокеты и файловые дескрипторы), связанные с текущим потоком.

### flush() {#flush--}
```
public void flush()
```


Очищает все буферы этого потока и заставляет любые буферизованные данные записаться в нижележащее устройство.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Записывает последовательность байтов в сжимающий поток и перемещает текущую позицию в этом потоке на количество записанных байтов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| буфер | byte[] | массив байтов. Этот метод копирует count байтов из buffer в текущий поток |
| смещение | int | нуль‑базовое смещение байта в buffer, с которого начинать копировать байты в текущий поток |
| количество | int | количество байтов, которое будет записано в текущий поток |

### write(int b) {#write-int-}
```
public void write(int b)
```


Записывает указанный байт в этот выходной поток. Общий контракт для `write` заключается в том, что один байт записывается в выходной поток. Байт, который будет записан, представляет собой восемь младших бит аргумента `b`. 24 старших бита `b` игнорируются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| b | int | `byte` |

