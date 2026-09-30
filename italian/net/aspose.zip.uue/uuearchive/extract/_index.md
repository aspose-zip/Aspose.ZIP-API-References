---
title: "UueArchive.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo UueArchive. Estrae l'archivio nello stream fornito"
type: docs
weight: 40
url: /it/net/aspose.zip.uue/uuearchive/extract/
---
## Extract(Stream) {#extract_1}

Estrae l'archivio nello stream fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Stream | Stream di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentException | *destination* non supporta la scrittura. |

## Esempi

```csharp
using (var archive = new UueArchive("archive.uue"))
{
     archive.Extract(httpResponseStream);
}
```

### Vedi anche

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Estrae l'archivio nel file specificato dal percorso.

```csharp
public FileInfo Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |

### Valore restituito

Informazioni sul file estratto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| FileNotFoundException | Il file non è stato trovato. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| InvalidDataException | Generato quando i dati non sono validi o sono corrotti. |

### Vedi anche

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


