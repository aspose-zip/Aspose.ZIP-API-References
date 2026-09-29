---
title: "FastLZOutputStream"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Un wrapper de flux qui compresse les données avec FastLZ."
type: docs
weight: 68
url: /fr/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Un wrapper de flux qui compresse les données avec FastLZ. Implémente le motif décorateur.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Initialise une nouvelle instance de la classe FastLZStream préparée pour la compression. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | Ferme le flux actuel et libère toutes les ressources (telles que les sockets et les poignées de fichiers) associées au flux actuel. |
| [flush()](#flush--) | Efface tous les tampons de ce flux et provoque l'écriture de toutes les données tamponnées sur le dispositif sous-jacent. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Écrit une séquence d'octets dans le flux de compression et avance la position actuelle dans ce flux du nombre d'octets écrits. |
| [write(int b)](#write-int-) | Écrit l'octet spécifié dans ce flux de sortie. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Initialise une nouvelle instance de la classe FastLZStream préparée pour la compression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | le flux pour enregistrer les données compressées |
| compressionLevel | int | utilisez 1 pour une compression plus rapide, utilisez 2 pour un meilleur taux de compression |

### close() {#close--}
```
public void close()
```


Ferme le flux actuel et libère toutes les ressources (telles que les sockets et les poignées de fichiers) associées au flux actuel.

### flush() {#flush--}
```
public void flush()
```


Efface tous les tampons de ce flux et provoque l'écriture de toutes les données tamponnées sur le dispositif sous-jacent.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Écrit une séquence d'octets dans le flux de compression et avance la position actuelle dans ce flux du nombre d'octets écrits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| buffer | byte[] | un tableau d'octets. Cette méthode copie count octets du tampon vers le flux actuel |
| offset | int | le décalage d'octet basé sur zéro dans le tampon à partir duquel commencer à copier les octets vers le flux actuel |
| count | int | le nombre d'octets à écrire dans le flux actuel |

### write(int b) {#write-int-}
```
public void write(int b)
```


Écrit l'octet spécifié dans ce flux de sortie. Le contrat général pour `write` est qu'un octet est écrit dans le flux de sortie. L'octet à écrire correspond aux huit bits de poids faible de l'argument `b`. Les 24 bits de poids fort de `b` sont ignorés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| b | int | le `byte` |

