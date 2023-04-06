---
title: Bzip2Archive.Extract
second_title: Riferimento API Aspose.ZIP per .NET
description: Bzip2Archive metodo. Estrae larchivio nel flusso fornito.
type: docs
weight: 30
url: /it/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

Estrae l'archivio nel flusso fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destination | Stream | Flusso di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destination* non supporta la scrittura. |

### Esempi

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)


