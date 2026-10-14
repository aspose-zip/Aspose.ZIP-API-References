---
title: "UueArchive.Open"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo UueArchive. Apre l'archivio per la decodifica e fornisce uno stream con il contenuto dell'archivio."
type: docs
weight: 60
url: /it/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Apre l'archivio per la decodifica e fornisce uno stream con il contenuto dell'archivio.

```csharp
public Stream Open()
```

### Valore restituito

Lo stream che rappresenta il contenuto dell'archivio.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

Leggi dallo stream per ottenere il contenuto originale di un file. Vedi la sezione esempi.

## Esempi

Utilizzo:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 e versioni successive - usa il metodo Stream.CopyTo:

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

### Vedi anche

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


