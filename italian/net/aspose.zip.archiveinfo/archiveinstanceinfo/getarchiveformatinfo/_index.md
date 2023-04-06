---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveInstanceInfo metodo. Ottiene informazioni sul formato dellarchivio.
type: docs
weight: 50
url: /it/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Ottiene informazioni sul formato dell'archivio.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome file del file di archivio. |

### Valore di ritorno

Informazioni sul formato dell'archivio o null se il formato non è stato rilevato.

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

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* spazio dei nomi [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assemblea [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Ottiene informazioni sul formato dell'archivio.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso del file di archivio. |

### Valore di ritorno

Informazioni sul formato dell'archivio o null se il formato non è stato rilevato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *stream* è zero. |
| ArgumentException | *stream* non è ricercabile. |

### Guarda anche

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* spazio dei nomi [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assemblea [Aspose.Zip](../../../)


