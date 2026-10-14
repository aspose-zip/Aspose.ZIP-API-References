---
title: "TarArchive.SaveZstandard"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo TarArchive. Salva l'archivio nello stream con compressione Zstandard"
type: docs
weight: 220
url: /it/net/aspose.zip.tar/tararchive/savezstandard/
---
## SaveZstandard(Stream, TarFormat?) {#savezstandard}

Salva l'archivio nello stream con compressione Zstandard.

```csharp
public void SaveZstandard(Stream output, TarFormat? format = default)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Stream di destinazione. |
| formato | Nullable`1 | Definisce il formato dell'intestazione tar. Il valore null sarà trattato come USTar quando possibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è nullo. |
| ArgumentException | *output* non è scrivibile. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere usato |
| IOException | Si è verificato un errore di I/O. |

## Osservazioni

*output* must be writable.

## Esempi

```csharp
using (FileStream result = File.OpenWrite("result.tar.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
        }
    }
}
```

### Vedi anche

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZstandard(string, TarFormat?) {#savezstandard_1}

Salva l'archivio nel file indicato dal percorso con compressione Zstandard.

```csharp
public void SaveZstandard(string path, TarFormat? format = default)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| formato | Nullable`1 | Definisce il formato dell'intestazione tar. Il valore null sarà trattato come USTar quando possibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| UnauthorizedAccessException | Il chiamante non dispone dell'autorizzazione richiesta. -oppure- *path* specifica un file o una directory di sola lettura. |
| ArgumentException | *path* è una stringa di lunghezza zero, contiene solo spazi bianchi, o contiene uno o più caratteri non validi come definiti da InvalidPathChars. |
| ArgumentNullException | *path* è nullo. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| DirectoryNotFoundException | Il *path* specificato non è valido, (ad esempio, si trova su un'unità non mappata). |
| NotSupportedException | *path* è in un formato non valido. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere usato |

## Esempi

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.tar.zst");
    }
}
```

### Vedi anche

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


