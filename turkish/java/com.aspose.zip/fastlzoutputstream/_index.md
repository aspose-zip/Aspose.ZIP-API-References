---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP for Java API Referansı"
description: "FastLZ ile verileri sıkıştıran bir akış sarmalayıcısı."
type: docs
weight: 68
url: /tr/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

FastLZ ile veri sıkıştıran bir akış sarmalayıcı. Dekoratör desenini uygular.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Sıkıştırma için hazırlanmış FastLZStream sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | Mevcut akışı kapatır ve mevcut akışla ilişkili tüm kaynakları (soketler ve dosya tutamaçları gibi) serbest bırakır. |
| [flush()](#flush--) | Bu akış için tüm tamponları temizler ve tamponlanmış verilerin temel cihaza yazılmasını sağlar. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Sıkıştırma akışına bir bayt dizisi yazar ve bu akıştaki mevcut konumu yazılan bayt sayısı kadar ilerletir. |
| [write(int b)](#write-int-) | Belirtilen baytı bu çıktı akışına yazar. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Sıkıştırma için hazırlanmış FastLZStream sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | sıkıştırılmış veriyi kaydetmek için akış |
| compressionLevel | int | daha hızlı sıkıştırma için 1, daha iyi sıkıştırma oranı için 2 kullanın |

### close() {#close--}
```
public void close()
```


Mevcut akışı kapatır ve mevcut akışla ilişkili tüm kaynakları (soketler ve dosya tutamaçları gibi) serbest bırakır.

### flush() {#flush--}
```
public void flush()
```


Bu akış için tüm tamponları temizler ve tamponlanmış verilerin temel cihaza yazılmasını sağlar.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Sıkıştırma akışına bir bayt dizisi yazar ve bu akıştaki mevcut konumu yazılan bayt sayısı kadar ilerletir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| buffer | byte[] | bayt dizisi. Bu yöntem, tampondan mevcut akışa count bayt kopyalar |
| offset | int | tampondaki sıfır tabanlı bayt ofseti, baytların mevcut akışa kopyalanmaya başlanacağı yer |
| count | int | mevcut akışa yazılacak bayt sayısı |

### write(int b) {#write-int-}
```
public void write(int b)
```


Belirtilen baytı bu çıktı akışına yazar. `write` için genel sözleşme, bir baytın çıktı akışına yazılmasıdır. Yazılacak bayt, `b` argümanının düşük sekiz bitidir. `b` nin yüksek 24 biti yok sayılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| b | int | `byte` |

