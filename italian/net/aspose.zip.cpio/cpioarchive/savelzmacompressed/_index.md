---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo CpioArchive. Salva l'archivio nello stream con compressione LZMA"
type: docs
weight: 110
url: /it/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Salva l'archivio nello stream con compressione LZMA.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Stream di destinazione. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| NotSupportedException | Lo stream non supporta la scrittura, oppure lo stream è già chiuso. |

## Osservazioni

*output* must be writable.

Importante: l'archivio cpio viene composto e poi compresso all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

## Esempi

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Vedi anche

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Salva l'archivio nel file specificato dal percorso con compressione lzma.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentNullException | *path* è `null`. |
| Eccezione | Generata quando si verifica un errore di runtime. |
| DirectoryNotFoundException | Il percorso specificato non è valido, (ad esempio, è su un'unità non mappata). |
| IOException | Si è verificato un errore di I/O. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. |
| UnauthorizedAccessException | Il chiamante non dispone dell'autorizzazione richiesta. -oppure- *path* specifica un file o una directory di sola lettura. |

## Osservazioni

Importante: l'archivio cpio viene composto e poi compresso all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

## Esempi

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Vedi anche

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


