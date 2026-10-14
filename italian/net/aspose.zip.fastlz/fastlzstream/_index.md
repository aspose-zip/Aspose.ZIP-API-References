---
title: "Classe FastLZStream"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.FastLZ.FastLZStream. Un wrapper di stream che comprime i dati con FastLZ. Implementa il pattern decoratore"
type: docs
weight: 500
url: /it/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

Un wrapper di flusso che comprime i dati con FastLZ. Implementa il pattern decoratore.

```csharp
public class FastLZStream : Stream
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Inizializza una nuova istanza della classe `FastLZStream` preparata per la compressione. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Restituisce un valore che indica se lo stream corrente supporta la lettura. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Restituisce un valore che indica se lo stream corrente supporta lo spostamento. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Restituisce un valore che indica se lo stream corrente supporta la scrittura. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Restituisce la lunghezza in byte dello stream. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Ottiene o imposta la posizione all'interno dello stream corrente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Chiude lo stream corrente e rilascia tutte le risorse (come socket e handle di file) associate allo stream corrente. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Svuota tutti i buffer per questo stream e fa sì che i dati memorizzati vengano scritti sul dispositivo sottostante. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Legge una sequenza di byte dallo stream e avanza la posizione all'interno dello stream del numero di byte letti. Non supportato. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Imposta la posizione all'interno dello stream corrente. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Imposta la lunghezza dello stream corrente. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Scrive una sequenza di byte nello stream di compressione e avanza la posizione corrente all'interno di questo stream del numero di byte scritti. |

### Vedi anche

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


