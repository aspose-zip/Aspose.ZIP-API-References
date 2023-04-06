---
title: RarArchiveEntry.Open
second_title: Riferimento API Aspose.ZIP per .NET
description: RarArchiveEntry metodo. Apre la voce per lestrazione e fornisce un flusso con il contenuto della voce decompresso.
type: docs
weight: 100
url: /it/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso.

```csharp
public Stream Open(string password = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password facoltativa per la decrittazione. Può anche essere impostato all'interno[`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/). |

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

* class [RarArchiveEntry](../)
* spazio dei nomi [Aspose.Zip.Rar](../../rararchiveentry/)
* assemblea [Aspose.Zip](../../../)


