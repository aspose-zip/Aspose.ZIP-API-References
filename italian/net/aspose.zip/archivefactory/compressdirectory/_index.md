---
title: "ArchiveFactory.CompressDirectory"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo ArchiveFactory. Comprimi la directory specificata in un file archivio utilizzando il formato archivio fornito"
type: docs
weight: 10
url: /it/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Comprimi la directory specificata in un file archivio utilizzando il formato archivio fornito.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso della directory che verrà compressa. |
| outputFileName | String | Nome file di destinazione. |
| archiveFormat | ArchiveFormat | Il formato dell'archivio da creare (ad esempio, zip, rar, tar, ecc.). |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| DirectoryNotFoundException | Generato se la directory specificata da *path* non esiste. |
| ArgumentException | Generato se *path* è null o una stringa vuota. |
| NotSupportedException | Generato se il *archiveFormat* specificato non è supportato o riconosciuto. |
| ArgumentNullException | *path* è `null`. |

## Osservazioni

Questo metodo creerà un file archivio nella posizione specificata dal parametro *path*. Il nome del file archivio sarà tipicamente il nome della directory seguito dall'estensione file appropriata basata su *archiveFormat*. La directory stessa non viene modificata né eliminata.

## Esempi

Ecco un esempio di come utilizzare il metodo CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Questo creerà un file ZIP con il contenuto della directory al percorso specificato.
```

### Vedi anche

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


