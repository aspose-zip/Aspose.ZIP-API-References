---
title: "CpioArchive.SaveZstandard"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo CpioArchive. Salva l'archivio nello stream con compressione Zstandard"
type: docs
weight: 140
url: /it/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Salva l'archivio nello stream con compressione Zstandard.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Stream di destinazione. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è nullo. |
| ArgumentException | *output* non è scrivibile. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

*output* must be writable.

## Esempi

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Salva l'archivio nel file indicato dal percorso con compressione Zstandard.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentException | *path* è una stringa di lunghezza zero, contiene solo spazi bianchi, o contiene uno o più caratteri non validi come definiti da InvalidPathChars. |
| ArgumentNullException | *path* è `null`. |
| DirectoryNotFoundException | Il percorso specificato non è valido, (ad esempio, è su un'unità non mappata). |
| IOException | Si è verificato un errore di I/O. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. |
| UnauthorizedAccessException | Il chiamante non dispone dell'autorizzazione richiesta. -oppure- *path* specifica un file o una directory di sola lettura. |

## Esempi

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Vedi anche

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


