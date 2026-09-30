---
title: "Classe IsoArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Iso.IsoArchive. Rappresenta un archivio ISO ISO 9660"
type: docs
weight: 570
url: /it/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Rappresenta un archivio ISO (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Inizializza una nuova istanza della classe `IsoArchive` e crea un archivio ISO vuoto per aggiungere nuovi file e directory. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Inizializza una nuova istanza della classe `IsoArchive` e compone un elenco di voci che può essere estratto dall'archivio. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Inizializza una nuova istanza della classe `IsoArchive` e compone un elenco di voci che può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Ottiene le voci di tipo [`IsoEntry`](../isoentry/) che costituiscono l'archivio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Aggiunge una directory all'immagine ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Aggiunge un file all'immagine ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Aggiunge un file all'immagine ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Aggiunge un file all'immagine ISO. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Esegue operazioni definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Estrae tutte le voci nella directory specificata. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Salva l'immagine ISO nello stream specificato. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Salva l'immagine ISO nel percorso specificato. |

### Vedi anche

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


