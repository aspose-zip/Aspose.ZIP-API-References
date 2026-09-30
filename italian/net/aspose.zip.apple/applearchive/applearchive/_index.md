---
title: "AppleArchive.AppleArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore AppleArchive. Inizializza una nuova istanza della classe AppleArchive con le impostazioni utilizzate per le voci composte."
type: docs
weight: 10
url: /it/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Inizializza una nuova istanza della classe [`AppleArchive`](../) con le impostazioni utilizzate per le voci composte.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Impostazioni utilizzate durante la composizione di un nuovo Apple Archive. |

### Vedi anche

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`AppleArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La sorgente dell'archivio. |
| loadOptions | AppleArchiveLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è null. |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | *sourceStream* non è un Apple Archive valido. |
| EndOfStreamException | Il flusso termina inaspettatamente durante l'analisi delle voci dell'archivio. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi i metodi [`ExtractToDirectory`](../extracttodirectory/) e [`Open`](../../applearchiveentry/open/) per la decompressione.

### Vedi anche

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Inizializza una nuova istanza della classe [`AppleArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso completo o relativo al file di archivio. |
| loadOptions | AppleArchiveLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| FileNotFoundException | Il file non è stato trovato. |
| InvalidDataException | *path* non è un Apple Archive valido. |
| EndOfStreamException | Il flusso termina inaspettatamente durante l'analisi delle voci dell'archivio. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi i metodi [`ExtractToDirectory`](../extracttodirectory/) e [`Open`](../../applearchiveentry/open/) per la decompressione.

### Vedi anche

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


