---
title: XzArchive.XzArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: XzArchive costruttore. Inizializza una nuova istanza diXzArchive class e compone larchivio in formato xz.
type: docs
weight: 10
url: /it/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Inizializza una nuova istanza di[`XzArchive`](../) class e compone l'archivio in formato xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | XzArchiveSettings | Set di impostazioni di un particolare archivio xz: dimensione del dizionario, dimensione del blocco, tipo di controllo. |

### Guarda anche

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`XzArchive`](../) classe preparata per la decompressione.

```csharp
public XzArchive(Stream source)
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

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`XzArchive`](../) classe preparata per la decompressione.

```csharp
public XzArchive(string path)
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

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)


