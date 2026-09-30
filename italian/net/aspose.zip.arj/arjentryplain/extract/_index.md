---
title: "ArjEntryPlain.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo ArjEntryPlain. Estrae la voce nel file system usando il percorso fornito"
type: docs
weight: 40
url: /it/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Estrae la voce nel file system usando il percorso fornito.

```csharp
public FileInfo Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |

### Valore restituito

Le informazioni file di un file composto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo o vuoto. |
| ObjectDisposedException | Generata se l'archivio è stato eliminato. |
| FileNotFoundException | Il file non è stato trovato. |
| InvalidDataException | Mancata corrispondenza del checksum per intestazioni o dati. - oppure - L'archivio è corrotto. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. |
| NotImplementedException | Voce compressa con il metodo 4. |

## Esempi

Estrai due voci dall'archivio rar.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Vedi anche

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Estrae la voce dell'archivio ARJ in un file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo per memorizzare i dati decompressi. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Intestazioni dell'archivio e informazioni di servizio non sono state lette. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per aprire il *fileInfo*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *fileInfo* è nullo. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se l'archivio è stato eliminato. |
| InvalidDataException | Mancata corrispondenza del checksum per intestazioni o dati. - oppure - L'archivio è corrotto. |
| NotImplementedException | Voce compressa con il metodo 4. |

## Esempi

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Vedi anche

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Estrae la voce nello stream fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Stream | Stream di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destination* non supporta la scrittura. |
| InvalidDataException | Mancata corrispondenza del checksum per intestazioni o dati. - oppure - L'archivio è corrotto. |
| NotImplementedException | Voce compressa con il metodo 4. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se l'archivio è stato eliminato. |

### Vedi anche

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


