---
title: "GetFormatInfo"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: 
type: docs
weight: 20
url: /it/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Ottiene informazioni sul formato.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome file del file di archivio. |

### Valore restituito

Informazioni sul formato dell'archivio o null se il formato non è stato rilevato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *fileName* è null. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *fileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *fileName* è negato. |
| PathTooLongException | Il *fileName* specificato supera la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file a 260 caratteri. |
| NotSupportedException | Il file in *fileName* contiene due punti (:) nel mezzo della stringa. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |

### Vedi anche

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Ottiene informazioni sul formato.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Lo stream del file di archivio. |

### Valore restituito

Informazioni sul formato dell'archivio o null se il formato non è stato rilevato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *stream* è nullo. |
| ArgumentException | *stream* non è ricercabile. |

### Vedi anche

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Zip.dll -->
