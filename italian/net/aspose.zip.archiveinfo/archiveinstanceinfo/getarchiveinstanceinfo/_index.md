---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveInstanceInfo metodo. Ottiene informazioni sullistanza di archivio.
type: docs
weight: 10
url: /it/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Ottiene informazioni sull'istanza di archivio.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome file del file di archivio. |

### Valore di ritorno

Informazioni sull'istanza di archivio o null se il formato non è stato rilevato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *fileName* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*fileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*fileName* è negato. |
| PathTooLongException | Il specificato*fileName* supera la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*fileName* contiene i due punti (:) al centro della stringa. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |

### Guarda anche

* class [ArchiveInstanceInfo](../)
* spazio dei nomi [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assemblea [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Ottiene informazioni sull'istanza di archivio.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso del file di archivio. |

### Valore di ritorno

Informazioni sull'istanza di archivio o null se il formato non è stato rilevato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *stream* è zero. |
| ArgumentException | *stream* non è ricercabile. |

### Guarda anche

* class [ArchiveInstanceInfo](../)
* spazio dei nomi [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assemblea [Aspose.Zip](../../../)


