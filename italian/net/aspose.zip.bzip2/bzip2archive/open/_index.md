---
title: Open
second_title: Riferimento API Aspose.ZIP per .NET
description: Apre larchivio per lestrazione e fornisce uno stream con il contenuto dellarchivio.
type: docs
weight: 40
url: /it/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Apre l'archivio per l'estrazione e fornisce uno stream con il contenuto dell'archivio.

```csharp
public Stream Open()
```

### Valore di ritorno

Il flusso che rappresenta il contenuto dell'archivio.

### Osservazioni

Leggi dal flusso per ottenere il contenuto originale del file. Vedere la sezione esempi.

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
Stream decompressed = archive.Open();
```

### Guarda anche

* class [Bzip2Archive](../../bzip2archive)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive)
* assemblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->