---
title: ZArchive.ZArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: ZArchive costruttore. Inizializza una nuova istanza diZArchive classe preparata per la compressione.
type: docs
weight: 10
url: /it/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Inizializza una nuova istanza di[`ZArchive`](../) classe preparata per la compressione.

```csharp
public ZArchive()
```

### Guarda anche

* class [ZArchive](../)
* spazio dei nomi [Aspose.Zip.Z](../../zarchive/)
* assemblea [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`ZArchive`](../) classe preparata per la decompressione.

```csharp
public ZArchive(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | La fonte dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *source* non è ricercabile. |
| ArgumentNullException | *source* è zero. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Extract`](../extract/) metodo per decomprimere.

### Guarda anche

* class [ZArchive](../)
* spazio dei nomi [Aspose.Zip.Z](../../zarchive/)
* assemblea [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`ZArchive`](../) classe preparata per la decompressione.

```csharp
public ZArchive(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Percorso alla fonte dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Extract`](../extract/) metodo per decomprimere.

### Guarda anche

* class [ZArchive](../)
* spazio dei nomi [Aspose.Zip.Z](../../zarchive/)
* assemblea [Aspose.Zip](../../../)


