---
title: "CancellationFlag"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Le drapeau qui permet l'annulation des opérations."
type: docs
weight: 54
url: /fr/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Le drapeau qui permet l'annulation des opérations.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Construit une instance de CancellationFlag. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [cancel()](#cancel--) | Annule l'opération associée à cette instance de [CancellationFlag](../../com.aspose.zip/cancellationflag). |
| [cancelAfter(long delay)](#cancelAfter-long-) | Annule l'opération après un délai spécifié en millisecondes. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Annule l'opération après un délai spécifié dans l'unité de temps donnée. |
| [close()](#close--) | Ferme l'instance de [CancellationFlag](../../com.aspose.zip/cancellationflag) et libère toutes les ressources qui y sont associées. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Construit une instance de CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


Annule l'opération associée à cette instance de [CancellationFlag](../../com.aspose.zip/cancellationflag).

Si l'opération est déjà annulée, cette méthode ne fait rien.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Annule l'opération après un délai spécifié en millisecondes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| délai | long | Le délai en millisecondes après lequel l'opération sera annulée. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Annule l'opération après un délai spécifié dans l'unité de temps donnée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| délai | long | Le délai après lequel l'opération sera annulée. |
| unité | java.util.concurrent.TimeUnit | L'unité de temps du paramètre de délai. |

### close() {#close--}
```
public void close()
```


Ferme l'instance de [CancellationFlag](../../com.aspose.zip/cancellationflag) et libère toutes les ressources qui y sont associées.

