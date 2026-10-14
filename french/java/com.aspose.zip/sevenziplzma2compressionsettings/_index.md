---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la méthode de compression LZMA2 dans une archive 7z."
type: docs
weight: 114
url: /fr/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Paramètres pour la méthode de compression LZMA2 dans une archive 7z.

LZMA2 prend en charge plusieurs exécutions de données LZMA compressées et de données non compressées.

Voir plus : [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Instancie les paramètres pour la méthode de compression LZMA2 dans une archive 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Instancie les paramètres pour la méthode de compression LZMA2 dans une archive 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Instancie les paramètres pour la méthode de compression LZMA2 dans une archive 7z. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Obtient le nombre de threads de compression. |
| [getDictionarySize()](#getDictionarySize--) | La taille du dictionnaire (tampon d'historique) indique combien d'octets des données non compressées récemment traitées sont conservés en mémoire. |
| [getFastBytes()](#getFastBytes--) | Obtient le nombre de contrôle des octets rapides utilisés par le compresseur LZMA2. |
| [getMethod()](#getMethod--) | Obtient la méthode de compression ou de décompression. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Définit le nombre de threads de compression. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Instancie les paramètres pour la méthode de compression LZMA2 dans une archive 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Instancie les paramètres pour la méthode de compression LZMA2 dans une archive 7z.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | dictionarySize | int | la taille du tampon d'historique, doit être comprise entre 4096 et 1073741824. |

Plus le dictionnaire est grand, généralement le taux de compression est meilleur - mais les dictionnaires plus grands que les données non compressées sont un gaspillage de RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Instancie les paramètres pour la méthode de compression LZMA2 dans une archive 7z.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | dictionarySize | int | la taille du tampon d'historique, doit être comprise entre 4096 et 1073741824. |

Plus le dictionnaire est grand, généralement le taux de compression est meilleur - mais les dictionnaires plus grands que les données non compressées sont un gaspillage de RAM. |
| fastBytes | int | contrôle le nombre d'octets rapides utilisés par les compresseurs LZMA2. Un nombre plus élevé d'octets rapides peut offrir un meilleur taux de compression au détriment de la vitesse de compression. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Obtient le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée.

**Returns:**
int - nombre de threads de compression
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


La taille du dictionnaire (tampon d'historique) indique combien d'octets des données non compressées récemment traitées sont conservés en mémoire.

**Returns:**
int - taille du dictionnaire (tampon d'historique)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Obtient le nombre de contrôle des octets rapides utilisés par le compresseur LZMA2.

**Returns:**
int - le nombre de contrôle des octets rapides utilisés par le compresseur LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Obtient la méthode de compression ou de décompression.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Définit le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | nombre de threads de compression. |

Ne définissez pas ce nombre supérieur au nombre de cœurs CPU. |

