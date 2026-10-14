---
title: "LzmaArchiveSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres de l'archive lzma."
type: docs
weight: 87
url: /fr/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Paramètres de l'archive lzma.

L'algorithme Lempel\\u2013Ziv\\u2013Markov chain (LZMA) est un algorithme utilisé pour effectuer une compression de données sans perte. Cet algorithme utilise un schéma de compression par dictionnaire quelque peu similaire à l'algorithme LZ77 et offre un taux de compression élevé ainsi qu'une taille de dictionnaire de compression variable.

Voir plus: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Initialise une nouvelle instance de la classe [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) avec une taille de dictionnaire par défaut, égale à 16 mégaoctets, un nombre d'octets rapides égal à 32 et des bits de contexte littéral égaux à 3. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [getDictionarySize()](#getDictionarySize--) | La taille du dictionnaire (tampon d'historique) indique combien d'octets des données non compressées récemment traitées sont conservés en mémoire. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Obtient le nombre de bits de contexte littéral. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Obtient le nombre d'octets utilisés pour la recherche de correspondances rapides dans l'algorithme LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | La taille du dictionnaire (tampon d'historique) indique combien d'octets des données non compressées récemment traitées sont conservés en mémoire. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Définit le nombre de bits de contexte littéral. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Définit le nombre d'octets utilisés pour la recherche de correspondances rapides dans l'algorithme LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Initialise une nouvelle instance de la classe [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) avec une taille de dictionnaire par défaut, égale à 16 mégaoctets, un nombre d'octets rapides égal à 32 et des bits de contexte littéral égaux à 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


La taille du dictionnaire (tampon d'historique) indique combien d'octets des données non compressées récemment traitées sont conservés en mémoire. Si elle n'est pas définie, elle sera choisie en fonction de la taille de l'entrée.

Plus le dictionnaire est grand, généralement le taux de compression est meilleur – mais les dictionnaires plus grands que les données non compressées sont un gaspillage de RAM. La taille du dictionnaire d'une archive LZMA doit être soit une puissance de deux (2^n), soit trois fois une puissance de deux (3\\*2^n).

**Returns:**
int - taille du dictionnaire (tampon d'historique).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Obtient le nombre de bits de contexte littéral.

Les bits de contexte littéral définissent combien des bits les plus significatifs du précédent octet non compressé sont utilisés pour prédire les bits du prochain octet littéral. Doivent être compris entre 0 et 8.

**Returns:**
int - le nombre de bits de contexte littéral.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Obtient le nombre d'octets utilisés pour la recherche de correspondances rapides dans l'algorithme LZMA.

Une valeur plus élevée permet au compresseur de rechercher des correspondances plus longues, ce qui peut améliorer légèrement le taux de compression mais ralentit la compression.

**Returns:**
int - le nombre d'octets utilisés pour la recherche de correspondance rapide dans l'algorithme LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Définit un événement qui est déclenché lorsqu'une partie du flux brut est compressée.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

