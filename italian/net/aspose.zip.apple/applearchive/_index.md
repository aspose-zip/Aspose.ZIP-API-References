---
title: "Classe AppleArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Apple.AppleArchive. Questa classe rappresenta un file Apple Archive .aar. Usala per creare file Apple Archive"
type: docs
weight: 60
url: /it/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Questa classe rappresenta un file Apple Archive (.aar). Usala per creare file Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Inizializza una nuova istanza della classe `AppleArchive` con le impostazioni usate per le voci composte. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Inizializza una nuova istanza della classe `AppleArchive` e compone un elenco di voci che può essere estratto dall'archivio. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Inizializza una nuova istanza della classe `AppleArchive` e compone un elenco di voci che può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Ottiene le voci che costituiscono l'archivio. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Restituisce un valore che indica se l'archivio utilizza la compressione solida. In modalità solida, tutti i dati delle voci sono compressi in un unico flusso e l'estrazione di singole voci non è disponibile. Usa [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) invece. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Ottiene le impostazioni usate per le nuove voci composte. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory specificata. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Crea una singola voce all'interno dell'archivio. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Esegue operazioni definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Estrae tutti i file dell'archivio nella directory fornita. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Salva l'archivio in un file di destinazione fornito. |

## Osservazioni

Apple e Apple Archive sono marchi registrati di Apple Inc.

### Vedi anche

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


