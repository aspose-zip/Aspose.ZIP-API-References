---
title: "FastLZStream.Read"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "FastLZStream metodo. Legge una sequenza di byte dallo stream e avanza la posizione all'interno dello stream del numero di byte letti. Non supportato"
type: docs
weight: 90
url: /it/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Legge una sequenza di byte dallo stream e avanza la posizione all'interno dello stream del numero di byte letti. Non supportato.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| buffer | Byte[] | Un array di byte. Quando questo metodo restituisce, il buffer contiene l'array di byte specificato con i valori compresi tra offset e (offset + count - 1) sostituiti dai byte letti dalla sorgente corrente. |
| offset | Int32 | L'offset di byte basato su zero in buffer a partire dal quale iniziare a memorizzare i dati letti dal flusso corrente. |
| count | Int32 | Il numero massimo di byte da leggere dal flusso corrente. |

### Valore restituito

Il numero totale di byte letti nel buffer. Questo può essere inferiore al numero di byte richiesti se non sono attualmente disponibili tanti byte, o zero (0) se è stato raggiunto la fine dello stream.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| NotSupportedException | L'operazione non è supportata. |

### Vedi anche

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


