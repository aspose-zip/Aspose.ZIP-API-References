---
title: ArchiveEntry.Open
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveEntry metodo. Apre la voce per lestrazione e fornisce un flusso con il contenuto della voce decompresso.
type: docs
weight: 110
url: /it/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso.

```csharp
public Stream Open(string password = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password facoltativa per la decrittazione. |

### Valore di ritorno

Il flusso che rappresenta il contenuto della voce.

### Osservazioni

Leggi dal flusso per ottenere il contenuto originale del file. Vedere la sezione degli esempi.

### Esempi

Utilizzo:

.NET 4.0 e versioni successive: utilizzare il metodo Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 e precedenti - copia i byte manualmente:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Guarda anche

* class [ArchiveEntry](../)
* spazio dei nomi [Aspose.Zip](../../archiveentry/)
* assemblea [Aspose.Zip](../../../)


