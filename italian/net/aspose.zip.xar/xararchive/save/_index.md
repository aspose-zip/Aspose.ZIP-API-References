---
title: "XarArchive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo XarArchive. Salva l'archivio nel file di destinazione fornito"
type: docs
weight: 80
url: /it/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| saveOptions | XarSaveOptions | Opzioni per salvare l'archivio xar. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationFileName* è nullo. |
| InvalidOperationException | Impossibile modificare l'archivio xar. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. |
| UnauthorizedAccessException | *destinationFileName* specifica un file in sola lettura. - o - *destinationFileName* specifica una directory. - o - Il chiamante non dispone dell'autorizzazione necessaria. |

### Vedi anche

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Stream di destinazione. |
| saveOptions | XarSaveOptions | Opzioni per salvare l'archivio xar. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è nullo. |
| ArgumentException | *output* non è scrivibile/leggibile o non è ricercabile. |
| InvalidOperationException | Impossibile modificare l'archivio xar. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

### Vedi anche

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


