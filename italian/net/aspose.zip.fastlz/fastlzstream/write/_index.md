---
title: "FastLZStream.Write"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "FastLZStream metodo. Scrive una sequenza di byte nello stream di compressione e avanza la posizione corrente all'interno di questo stream del numero di byte scritti"
type: docs
weight: 120
url: /it/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Scrive una sequenza di byte nello stream di compressione e avanza la posizione corrente all'interno di questo stream del numero di byte scritti.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| buffer | Byte[] | Un array di byte. Questo metodo copia count byte da buffer al flusso corrente. |
| offset | Int32 | L'offset di byte basato su zero in buffer a partire dal quale iniziare a copiare i byte nel flusso corrente. |
| count | Int32 | Il numero di byte da scrivere nel flusso corrente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | Generata se lo stream è stato eliminato. |
| ArgumentNullException | *buffer* è `null`. |

### Vedi anche

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


